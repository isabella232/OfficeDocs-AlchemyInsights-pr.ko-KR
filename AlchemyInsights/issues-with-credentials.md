---
title: 자격 증명 관련 문제
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
- "9004330"
- "7723"
ms.openlocfilehash: 975d4850c1ecffae786dd19b7f4363e0c95378cff4f3ae6bb1968af33ef810b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986825"
---
# <a name="issues-with-credentials"></a>자격 증명 관련 문제

[Microsoft ID 플랫폼 및 OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 클라이언트 자격 증명 흐름에서는 OAuth 2.0 클라이언트 자격 증명에 대해 직접 프로그래밍하는 방법을 설명하고 흐름을 부여합니다.

**응용 프로그램의 암호 또는 인증서 자격 증명을 관리하는 방법**

Azure CLI에서 az 광고 앱 자격 [증명을](https://docs.microsoft.com/cli/azure/ad/app/credential) 사용하여 응용 프로그램의 암호 또는 인증서 자격 증명을 삭제, 목록 또는 다시 설정할 수 있습니다.

**사용자는 어떻게 암호를 재설정하나요?**

사용자가 암호를 [다시](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) 설정하려면 먼저 셀프 서비스 암호 재설정을 등록해야 합니다. 사용자가 등록한 후 이 문서의 지침에 따라 암호를 재설정할 수 있습니다. [직장](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)또는 학교 암호 다시 설정 .

**사용자는 암호를 어떻게 변경하나요?**

사용자는 이 문서의 단계에 따라 암호를 변경할 수 있습니다. 암호 변경 [방법.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)
또한 2단계 인증을 위해 앱 [암호를 관리할 수 있습니다.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)

**사용자가 암호를 변경하거나 재설정할 때 오류가 발생했습니다.**

이 링크는 사용자가 암호를 다시 설정하려고 할 때 발생할 수 있는 일반적인 문제( 일반적인 문제 및 해결 방법)에 [대한 정보를 제공합니다.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**사용자의 암호를 다시 설정하는 데 문제가 있습니다.**

- 암호를 재설정할 권한이 있는지 확인 *전역, 암호 및 사용자 관리자만 사용자 암호를 재설정할 수 있습니다.* 전역 관리자는 권한이 부여된 다른 관리자의 암호를 다시 설정할 수도 있습니다.

- 라이선스 요구 사항을 이해해야 합니다.

  - 조직에 라이선스가 하나 이상 할당되어 있어야 합니다.
    - **클라우드 전용 사용자** - 모든 Office 365(O365) 유료 SKU 또는 Azure AD Basic
    - **클라우드 및/또는** 사내 사용자 - Azure AD Premium P1 P2, EMS(Enterprise Mobility + Security) 또는 SPE(Secure Productive Enterprise)
    - 라이선스 요구 사항에 대한 자세한 내용은 Azure AD 셀프 서비스 암호 재설정에 대한 라이선스 [요구 사항을 참조하세요.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- 사용자의 암호를 다시 설정하기 위해 Azure AD에서 사용자를 찾아야 합니다. 그런 다음 해당 사용자의 개요 블레이드에서 "암호 재설정" 단추를 클릭합니다.

**암호 재설정 단추가 회색으로 표시되어 있습니다.**

이 사용자의 암호를 다시  설정할 수 있는 권한이 없습니다. *전역, 암호 및 사용자 관리자만 사용자 암호를 재설정할 수 있습니다.* 전역 관리자는 권한이 부여된 다른 관리자의 암호를 다시 설정할 수도 있습니다.

**암호 재설정 블레이드가 표시되지 않습니다.**

암호를 재설정할 수 있는 권한이 없습니다. *전역, 암호 및 사용자 관리자만 사용자 암호를 재설정할 수 있습니다.* 전역 관리자는 권한이 부여된 다른 관리자의 암호를 다시 설정할 수도 있습니다.

**암호 재설정 시에는 프레미스 통합 블레이드가 볼 수 없습니다.**

- 사내 통합 블레이드는 하이브리드 환경에서만 나타납니다. 즉, 암호 쓰기 저장을 사용하여 On-premises 사용자의 암호를 조작할 수 있습니다.

- 다음 경우 이 블레이드가 표시되지 않습니다.

  - 암호 쓰기 저장을 사용하고 있지 않습니다.
  - 암호 쓰기 저장 설치/연결에 문제가 있습니다.
  - Azure AD 설치/연결에 문제가 커넥트
  - 암호 쓰기 저장 관련 문제에 대한 자세한 문제 해결 단계는 암호 쓰기 저장 [문제 해결을 참조하세요.](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**사용자 암호를 다시 설정하는 방법을 모르는 경우**

1. Azure Portal에 적절한 관리자로 로그인합니다.
2. 사용자 및 그룹 **블레이드로 이동하여** 모든 사용자를 **선택합니다.**
3. 목록에서 사용자를 선택합니다.
4. 선택한 사용자의 경우 개요를 선택한 다음 명령 표시줄에서 암호 **재설정을 선택합니다.**
5. 암호 **다시 설정 단추를** 선택하고 화면의 지침을 따릅니다.
    - Azure Portal에서 암호 **쓰기** 저장을 지원하는 데만 수행되는 재설정입니다.

**Office 365 관리자 포털 또는 모바일 응용 프로그램에서 Office 365 사용자 암호를 다시 설정했지만 사용자가 여전히 로그인할 수 없습니다.**

암호 쓰기 저장은 이 포털에서 지원되지 않습니다. Azure Portal에서 사용자 암호를 다시 초기화합니다.
