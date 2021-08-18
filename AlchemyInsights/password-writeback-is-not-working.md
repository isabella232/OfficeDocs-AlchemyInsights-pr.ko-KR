---
title: 암호 쓰기 저장이 작동하지 않습니다.
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
- "9004595"
- "8210"
ms.openlocfilehash: 679dea6d488cf74f51baee2b3b498dc64b95530e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324929"
---
# <a name="password-writeback-is-not-working"></a>암호 쓰기 저장이 작동하지 않습니다.

**암호 쓰기 저장 구성에 문제가 있습니다.**

- 암호 쓰기 저장은 고급 기능입니다.
- 라이선스 요구 사항을 이해해야 합니다.
  - 조직에 라이선스가 하나 이상 할당되어 있어야 합니다.
  - **클라우드 전용 사용자** - 모든 Office 365(O365) 유료 SKU 또는 Azure AD Basic
  - **클라우드 및/또는** 사내 사용자 - Azure AD Premium P1 P2, EMS(Enterprise Mobility + Security) 또는 SPE(Secure Productive Enterprise)
    - 라이선스 요구 사항에 대한 자세한 내용은 Azure AD 셀프 서비스 암호 재설정에 대한 라이선스 [요구 사항을 참조하세요.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- 적절한 라이선스 중 하나를 사용하려면 관리자 계정과 테스트 사용자 계정이 하나 이상 있습니다.
- 암호 쓰기 저장이 커넥트 Azure AD Emulator 도메인 컨트롤러 서버에 연결해야 합니다. Active Directory 동기화 커넥트 속성을 마우스 오른쪽 단추로 클릭한 다음  디렉터리 파티션 구성을 선택하여 기본 도메인 컨트롤러를 사용하도록 Azure AD 2013을 구성할 **수 있습니다.** 이 섹션에서 도메인  컨트롤러 연결 설정 섹션을 찾아 기본 설정 도메인 컨트롤러만 사용이라는 **확인란을 선택합니다.**
    **참고:기본** 설정 DC가 PDC 에뮬레이터가 아닌 경우 Azure AD 커넥트 암호 쓰기 저장을 위해 PDC에 계속 도달합니다.
- 암호 재설정이 구성되고 테넌트에서 사용하도록 설정되었습니다. 자세한 내용은 사용자가 Azure AD 암호를 [재설정할 수 있도록 설정을 참조하세요.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- 암호 쓰기 저장을 사용하도록 설정하는 데 사용되는 관리자 계정이 클라우드 관리자 계정(사내 AD가 아닌 Azure AD에서 생성)으로 설정되어 있는지 확인
- 최신 서비스 팩이 설치된 Windows Server 2008 R2, Windows Server 2012 또는 Windows Server 2012 R2를 실행하는 단일 또는 다중 포리스트 AD Windows Server 2012 배포가 있는 경우
- Azure AD 커넥트 도구가 설치되어 있으며 클라우드와의 동기화를 위해 AD 환경을 준비했습니다. 암호 쓰기 저장을 테스트하기 전에 먼저 Azure AD의 AD 및 Azure AD에서 전체 가져오기 및 전체 동기화를 커넥트.
- 자세한 내용은 [Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations) 2013에서 전체 동기화 및 전체 가져오기 작업을 커넥트

**암호 쓰기 저장 연결에 문제가 있습니다.**

1. 최신 버전의 Azure AD 서비스 다운로드 [및 커넥트](https://www.microsoft.com/download/details.aspx?id=47594)
2. 방화벽 구성: Azure AD 커넥트 도구(1.1.443 이상)에는 다음에 대한 아웃바운드 **HTTPS 액세스** 권한이 필요합니다.
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. 최소 2~3분 동안 유휴 연결을 유지하도록 허용

**암호 쓰기 저장에 여전히 문제가 있습니다.**

- 그래도 문제가 있는 경우 Azure AD 2013 도구에서 암호 쓰기 저장 서비스를 커넥트 다시 사용하도록 설정하세요.
- 자세한 내용은 암호 쓰기 저장을 사용하지 않도록 [설정하고 다시 사용하도록 설정하는 방법을 참조하세요.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
