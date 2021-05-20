---
title: Create user(사용자 만들기)
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 800baae2d748708d8cb7a5fb0e73fce5dcf455cb
ms.sourcegitcommit: 2d617ae59eed0ce8b571339ceefce6473c03b94c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52569737"
---
# <a name="create-user"></a>Create user(사용자 만들기)

**공지 사항:**

- [2021년 1월 4일부터 Google에서 WebView](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) 로그인 지원 사용이 더 이상 사용 안 됩니다. 호환성 테스트에 대한 [Google의](https://go.microsoft.com/fwlink/?linkid=2157323) 지침을 따라 앱이 영향을 받을 수 있는지 테스트합니다.
- 소비자 Google 계정을 사용하여 사용자에 로그인할 때 시스템 웹 보기 또는 시스템 브라우저를 사용하는지 확인 자세한 내용은 [Chrome 브라우저만 사용하여 응용 프로그램에 로그인하는 문제](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)를 참조하세요.

**Azure AD 디렉터리에서 새 사용자를 생성할 수 없습니다.**

1. 새 표준 사용자를 생성할 권한이 있는지 확인합니다. AD(Azure Active Directory)의 전역 관리자 또는 사용자 관리자 역할만 새 표준 사용자를 만들 수 있습니다. 이러한 역할 중 하나가 아닌 경우 관리자에게 이러한 역할 중 하나에 사용자를 추가하거나 새 사용자 계정을 만들도록 요청하세요.
1. 사용자 이름이 Azure AD에서 확인된 도메인에 있는지 확인합니다. Azure AD에 확인된 사용자 지정 도메인 이름이 없는 경우 *.onmicrosoft.com으로 끝나는 Azure AD 초기 도메인을 사용할 수 있습니다.
1. 사용자 이름이 온-프레미스 AD에서 Azure AD로 연합되지 않은 도메인에 있는지 확인하세요. 사내에서 연합된 도메인 이름으로 사용자를 클라우드에 추가할 수 없습니다.
1. 새 사용자에게 할당할 사용자 이름을 이미 가지고 있는 다른 사용자 또는 연락처가 없는지 확인합니다. 사용자 이름은 Azure AD 전반에서 고유해야 합니다.
1. Azure AD의 경우 [Azure AD 역할 및 관리자](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators)를 참조하세요.
1. Azure AD의 경우 [도메인 이름](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators)을 참조하세요.
1. [감사 로그 ](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators)을(를) 검토하여 작업을 수행한 사용자와 같이 최근에 생성되거나 삭제된 사용자에 대한 자세한 정보를 확인합니다.
1. 새 사용자를 추가하는 데 대한 자세한 내용은 Azure Portal을 사용하여 Azure AD에서 새 사용자 [만들기를 참조하세요.](/azure/active-directory/active-directory-users-create-azure-portal)
1. [Azure AD 관리 역할:](/azure/active-directory/active-directory-assign-admin-roles)Azure의 관리자 역할 Azure Active Directory
1. Azure [AD PowerShell을](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)사용하여 새 사용자를 만들 수 있습니다.
