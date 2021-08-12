---
title: PRT 문제 해결
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: fd285d1158d7b358e4c698cf6014422cc2fb536e1fbdf98630bebda359f9c553
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972722"
---
# <a name="troubleshoot-prt-issue"></a>PRT 문제 해결

모든 디바이스가 인증을 완료하려면 완전히 등록되어 있으며 양호한 상태로 PRT(주 새로 고침 토큰)를 획득할 수 있어야 합니다.

하이브리드 Azure AD 가입 등록 프로세스에서는 장치가 회사 네트워크에 있을 수 있습니다. 또한 VPN을 통해 작동하지만 몇 가지 주의가 있습니다. 원격 작업 환경에서 하이브리드 Azure AD 가입 등록 프로세스 문제 해결에 도움이 필요한 고객이 필요하다는 소식을 들었을 것입니다. 다음은 등록 프로세스 중에 '후드 아래'에 진행된 일의 분석입니다.

**클라우드 인증 환경(Azure AD 암호 해시 동기화 또는 통과 인증 사용)**

이 등록 흐름을 "동기화 조인"이라고도 합니다.

1. Windows 10 로그온할 때 SCP 레코드를 검색합니다.
    1. 장치는 먼저 레지스트리 [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]의 클라이언트 쪽 SCP에서 테넌트 정보를 검색합니다. 자세한 정보는 이 [문서](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)를 참조하세요.
    2. 오류가 발생하면 장치가 SCP(서비스 연결 지점)에서 테넌트 정보를 얻기 위해 사내 AD(Active Directory)와 통신합니다. SCP를 확인한 후 이 문서를 [참조하시기 바랍니다.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point) 

> [!NOTE]
> AD에서 SCP를 사용하도록 설정하고 초기 유효성 검사를 위해 클라이언트 쪽 SCP만 사용하는 것이 좋습니다.

2. Windows 10 Azure AD에 대해 인증하기 위해 시스템 컨텍스트에서 Azure AD와 통신을 합니다. 장치 등록 연결 테스트 스크립트를 사용하여 장치가 시스템 계정의 Microsoft 리소스에 액세스할 수 있는지 확인할 수 있습니다.

3. Windows 10 자체 서명된 인증서를 생성하고 해당 인증서를 컴퓨터 개체 아래에 사내 AD에 저장합니다. 이를 위해서는 도메인 컨트롤러에 대한 시야가 필요합니다.

4. 인증서가 있는 장치 개체는 Azure AD 앱을 통해 Azure AD에 커넥트. 동기화 주기는 기본적으로 30분마다 되지만 Azure AD 구성에 따라 커넥트. 자세한 내용은 이 문서를 [참조하세요.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. 이 단계에서 Azure Portal의 장치 블레이드에서 "보류 중" 상태의 주체 장치를 볼 수 있습니다.

6. 다음에 로그인하여 Windows 10 등록이 완료됩니다. 

> [!NOTE]
> VPN을 사용 중일 때 로그프 로그인 프로세스로 도메인 연결이 종료되면 수동으로 등록을 트리거할 수 있습니다.
 1. 관리자 프롬프트에서 로컬로 또는 PSExec을 통해 PC에 원격으로 dsregcmd /join을 발급합니다. 예를 들어 PsExec -s \\ win10client01 cmd, dsregcmd /join

 2. 하이브리드 가입 문제에 대한 자세한 내용은 장치 문제 [해결을 참조합니다.](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)
