---
title: 보류 중인 상태의 장치
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: 224e6e613c306b50e354930bcbe6f43f1c08528766cb6e681b0e9826b2d55a4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914009"
---
# <a name="device-in-pending-state"></a>보류 중인 상태의 장치

**선행 준비 사항:**

1. 장치 등록을 처음 설정하는 경우 [Azure AD를](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) 통해 디바이스를 다운로드하는 방법을 안내하는 Azure Active Directory(Azure AD)의 장치 관리 소개를 검토하세요.
2. 장치를 Azure AD에 직접 등록하고 Intune에 등록하는 경우 [Intune을](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) 구성하고 먼저 라이선스를 [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) 설정해야 합니다.
3. Azure AD 및 사내 AD에서 작업을 수행할 수 있는 권한이 부여되어 있는지 확인 Azure AD의 전역 관리자만 장치 등록 설정을 관리할 수 있습니다. 또한, 온-프레미스 Active Directory에서 자동 등록을 설정하는 경우 Active Directory 및 AD FS의 관리자(해당하는 경우)에게 문의해야 합니다.

하이브리드 Azure AD 가입 등록 프로세스에서는 장치가 회사 네트워크에 있을 수 있습니다. 또한 VPN을 통해 작동하지만 몇 가지 주의가 있습니다. 원격 작업 환경에서 하이브리드 Azure AD 가입 등록 프로세스 문제 해결에 도움이 필요한 고객이 필요하다는 소식을 들었습니다.

**클라우드 인증 환경(Azure AD 암호 해시 동기화 또는 통과 인증 사용)**

이 등록 흐름을 "동기화 조인"이라고도 합니다.

다음은 등록 프로세스 중에 발생하는 일의 분석입니다.

1. Windows 10 로그온할 때 SCP(서비스 연결 지점) 레코드를 검색합니다.

    1. 장치는 먼저 레지스트리 [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]의 클라이언트 쪽 SCP에서 테넌트 정보를 검색합니다. 자세한 내용은 문서를 [참조하세요.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)
    1. 오류가 발생하면 장치가 SCP에서 테넌트 정보를 얻기 위해 사내 Active Directory와 통신합니다. SCP를 확인하면 이 문서를 [참조합니다.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)

    > [!NOTE]
    > Active Directory에서 초기 유효성 검사를 위해 클라이언트 쪽 SCP만 사용하여 SCP를 사용하도록 설정하는 것이 좋습니다.

2. Windows 10 Azure AD에 대해 인증하기 위해 시스템 컨텍스트에서 Azure AD와 통신을 합니다.

    장치 등록 연결 테스트 스크립트를 사용하여 장치가 시스템 계정의 Microsoft 리소스에 액세스할 수 있는지 [확인할 수 있습니다.](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)

3. Windows 10 자체 서명된 인증서를 생성하고 해당 인증서를 컴퓨터 개체 아래에 사내 Active Directory에 저장합니다. 이를 위해서는 도메인 컨트롤러에 대한 시야가 필요합니다.

4. 인증서가 있는 장치 개체는 Azure AD 앱을 통해 Azure AD에 커넥트. 동기화 주기는 기본적으로 30분마다 되지만 Azure AD 구성에 따라 커넥트. 자세한 내용은 이 문서를 [참조하십시오.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. 이 단계에서 Azure Portal의 장치 블레이드에서 "**보류** 중인" 상태의 주체 장치를 볼 수 있습니다.

6. 다음에 로그인하여 Windows 10 등록이 완료됩니다.

    > [!NOTE]
    > VPN을 사용 중일 때 로그프/로그인이 도메인 연결을 종료하는 경우 수동으로 등록을 트리거할 수 있습니다. 이를 위해
    >
    > 관리자 `dsregcmd /join` 프롬프트에서 로컬로 발급하거나 PSExec을 통해 PC로 원격으로 발급합니다.
    >
    > 예: `PsExec -s \\win10client01 cmd, dsregcmd /join`

장치 등록에 Azure Active Directory 일반적인 문제는 [장치 FAQ 를 참조하세요.](https://docs.microsoft.com/azure/active-directory/devices/faq)
