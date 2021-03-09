---
title: 암호 재설정 문제
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: fe3a13acb0ba5c8872d7c0bb8c3961d83f7d3526
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568580"
---
# <a name="problems-resetting-password"></a>암호 재설정 문제

다음은 암호를 재설정할 때 직면할 수 있는 몇 가지 문제와 가능한 해결 방법입니다.

**다른 범주에서 다루지 않는 암호 재설정에 문제가 있습니다.**

-암호를 재설정할 권한이 부여된지 확인 전역, 암호 및 사용자 관리자만 사용자 암호를 재설정할 수 있습니다. 전역 관리자는 권한이 부여된 다른 관리자의 암호를 다시 설정할 수도 있습니다.
- 라이선스 요구 사항을 이해해야 합니다.
    - 조직에 라이선스가 하나 이상 할당되어 있어야 합니다.
        - 클라우드 전용 사용자 - Office 365(O365) 유료 SKU 또는 Azure AD Basic
        - 클라우드 및/또는 사내 사용자 - Azure AD Premium P1 또는 P2, EMS(Enterprise Mobility + Security) 또는 SPE(Secure Productive Enterprise)
        - 라이선스 요구 사항에 대한 자세한 내용은 Azure AD 셀프 서비스 암호 재설정에 대한 라이선스 요구 [사항을 참조하세요.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)

**설정한 암호 재설정 정책 테스트에 문제가 있습니다.**

- 최근에 적용된 정책은 모든 데이터 센터 및 끝점에서 복제하는 데 몇 분 정도 걸릴 수 있습니다. 데이터 센터와의 물리적 거리는 변경 내용이 적용되는 방식에도 영향을 미치게 됩니다.
- 관리자가 아닌 최종 사용자와 테스트하고 소수의 사용자로 파일럿을 실행합니다. Azure Portal에 구성된 정책은 관리자가 아닌 최종 사용자에게만 적용됩니다. Microsoft는 모든 Azure 관리자 역할에 대해 강력한 기본 2 게이트 암호 재설정 정책을 적용합니다(예: 전역 관리자, 헬프데스크 관리자, 암호 관리자 등).
    - 관리자의 정책에 [대해 자세히 알아보시고 을(를) 자세히 알아보아야 합니다.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)

**암호 재설정을 배포하고 싶지만 사용자가 추가 보안 정보를 등록할 수 있도록 하고 싶지 않습니다.**

사용자에 대한 데이터를 미리 채우면 사용자가 할 일도 없습니다! - 관리자는 조직에 암호 재설정을 롤아웃하기 전에 사용자의 전화 및 전자 메일 속성을 설정할 수 있습니다. API, PowerShell 또는 Azure AD Connect를 사용하여 이 작업을 할 수 있습니다. 자세한 내용은 다음을 참조하십시오.
- [사용자가 등록할 필요 없이 암호 재설정 배포](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [암호 재설정에 사용되는 데이터](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**암호 재설정 단추가 회색으로 표시되어 있습니다.**

이 사용자의 암호를 다시 설정할 수 있는 권한이 없습니다. 전역, 암호 및 사용자 관리자만 사용자 암호를 재설정할 수 있습니다. 전역 관리자는 권한이 부여된 다른 관리자의 암호를 다시 설정할 수도 있습니다.

**암호 재설정 블레이드가 표시되지 않습니다.**

암호를 재설정할 수 있는 권한이 없습니다. 전역, 암호 및 사용자 관리자만 사용자 암호를 재설정할 수 있습니다. 전역 관리자는 권한이 부여된 다른 관리자의 암호를 다시 설정할 수도 있습니다.

**암호 재설정 시에는 프레미스 통합 블레이드가 볼 수 없습니다.**

- 사내 통합 블레이드는 하이브리드 환경에서만 나타납니다. 즉, 암호 쓰기 저장을 사용하여 On-premises 사용자의 암호를 조작할 수 있습니다.
- 다음 경우 이 블레이드가 표시되지 않습니다.
    - 암호 쓰기 저장을 사용하고 있지 않습니다.
    - 암호 쓰기 저장 설치/연결에 문제가 있습니다.
    - Azure AD Connect의 설치/연결에 문제가 있습니다.
    - 암호 쓰기 저장 관련 문제에 대한 자세한 문제 해결 단계는 암호 쓰기 저장 문제 [해결 섹션을 참조하세요.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**사용자 암호를 다시 설정하는 방법을 모르는 경우**

1. Azure Portal에 적절한 관리자로 로그인합니다.
1. 사용자 및 그룹 블레이드로 이동하여 모든 사용자를 **선택합니다.**
1. 목록에서 사용자를 선택합니다.
1. 선택한 사용자에 대해 개요를 선택한 다음 명령 표시줄에서 암호 다시 설정을 **클릭합니다.**
1. 화면의 지시를 따릅니다.
    - Azure Portal에서 암호 쓰기 저장을 지원하는 데만 수행되는 재설정입니다.

**Office 365 관리 포털 또는 Office 365 모바일 응용 프로그램에서 사용자의 암호를 다시 설정했지만 사용자가 여전히 로그인할 수 없습니다.**

암호 쓰기 저장은 이 포털에서 지원되지 않습니다. Azure Portal에서 사용자 암호를 다시 portal.azure.com

