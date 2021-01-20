---
title: 사용자 문제 해결
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7813"
- "9004358"
ms.openlocfilehash: d9964e50bdea0c41ac14ab3783b579034b5f2c8c
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886908"
---
# <a name="announcements"></a>공지 사항

호환성 테스트 지침에 따라 앱이 영향을 받는지 테스트합니다. Google의 지침은 https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support에서 확인할 수 있습니다.

사용자 Google 계정으로 사용자를 로그인할 때 시스템 웹 보기 또는 시스템 브라우저를 사용해야 합니다. 자세한 내용은 [Chrome 브라우저만 사용하여 응용 프로그램에 로그인하는 문제](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)를 참조하세요.


**Azure AD 디렉터리에서 새 사용자를 생성할 수 없습니다.**

Azure AD에서 새 사용자를 생성할 수 없는 문제를 해결하려면 다음 단계를 수행하세요.

1. 새 표준 사용자를 생성할 권한이 있는지 확인합니다. Azure Active Directory(AD)의 전역 관리자 또는 사용자 관리자 역할만 새 표준 사용자를 생성할 수 있습니다. 이러한 역할 중 하나가 아닌 경우 관리자에게 이러한 역할 중 하나에 사용자를 추가하거나 새 사용자 계정을 만들도록 요청하세요.
2. 사용자 이름이 Azure AD에서 확인된 도메인에 있는지 확인합니다. Azure AD에 확인된 사용자 지정 도메인 이름이 없는 경우 *.onmicrosoft.com으로 끝나는 Azure AD 초기 도메인을 사용할 수 있습니다.
3. 사용자 이름이 온-프레미스 AD에서 Azure AD로 연합되지 않은 도메인에 있는지 확인하세요. 사내에서 연합된 도메인 이름으로 사용자를 클라우드에 추가할 수 없습니다.
4. 새 사용자에게 할당할 사용자 이름을 이미 가지고 있는 다른 사용자 또는 연락처가 없는지 확인합니다. 사용자 이름은 Azure AD 전반에서 고유해야 합니다.
5. Azure AD의 경우 [Azure AD 역할 및 관리자](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators)를 참조하세요.
6. Azure AD의 경우 [도메인 이름](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains)을 참조하세요.
7. [감사 로그 ](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit)을(를) 검토하여 작업을 수행한 사용자와 같이 최근에 생성되거나 삭제된 사용자에 대한 자세한 정보를 확인합니다.
8. 새 사용자 추가에 대한 자세한 내용은 [Azure 포털을 사용하여 Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)에서 새 사용자 생성을 참조하세요.
9. Azure AD의 관리자 역할 권한에 대한 자세한 내용은 [Azure AD 관리 역할](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)을 참조하세요.
10. Azure AD PowerShell을 사용하여 사용자를 생성하는 방법에 대한 자세한 내용은 [Azure AD PowerShell을 참조하여 새 사용자 ](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser)을(를) 생성하세요.

**자체 서비스 등록 문제**

셀프 서비스 등록과 관련된 문제를 해결하려면 다음 단계를 수행하세요.

1. 응용 프로그램과 함께 셀프 서비스 등록을 사용하려면 먼저 테넌트에 대해 셀프 서비스 등록을 사용하도록 설정하세요. 
2. 응용 프로그램이 셀프 서비스 등록을 지원하도록 하려면 해당 응용 프로그램을 사용자 흐름에 추가하세요. 다음에 해당 응용 프로그램의 로그인 페이지로 이동하면 **_계정이 없습니까? 계정을 하나 만들어 보세요!_* 라는 옵션이 나타납니다. 셀프 서비스 등록 프로세스가 시작됩니다.
3. Azure AD에서 셀프 서비스 등록을 사용하여 조직을 채우는 방법에 대한 자세한 내용은 [Azure AD ](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup)에 대한 셀프 서비스 등록을 참조하세요.
4. 사용자 흐름을 하나 이상의 응용 프로그램과 연결하면 해당 앱을 방문한 사용자가 사용자 흐름에 구성된 옵션을 사용하여 게스트 계정을 등록하고 얻을 수 있습니다. 게스트 계정 등록 및 가져오기에 대한 자세한 내용을 확인하기 위해 사용자는 [게스트 사용자에 대한 셀프 서비스 등록](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow)을 참고할 수 있습니다.

_ *외부 사용자 초대 관련 문제**

외부 사용자 초대와 관련된 문제를 해결하려면 다음 단계를 수행하세요.

사용자가 로그인하는 이름과 일치하는 전자 메일 주소로 사용자의 초대를 전송해야 합니다. 사용자의 프록시 전자 메일 주소로 초대장을 보내면 사용자가 해당 전자 메일 주소를 다시 사용할 수 없습니다. 자세한 내용은 [Azure ADB2B 설명서](https://docs.microsoft.com/azure/active-directory/external-identities/)를 참조하세요.

**사용자에게 라이선스를 할당할 수 없음**

사용자에게 라이선스 할당과 관련된 문제를 해결하려면 다음 단계를 수행하세요.

1. 사용자 라이선스를 관리하려면 전역 관리자, 라이선스 관리자 또는 사용자 관리자 등 필요한 관리자 역할 중 하나가 있는 계정을 사용해야 합니다. 사용자 블레이드의 **디렉터리 역할** 탭에서 사용자 역할을 확인할 수 있습니다.
2. Azure 포털을 사용하고 있는데 라이선스 할당에 실패하면 오른쪽 상단 모서리에 있는 알림을 클릭합니다. 그러면 무엇이 잘못되었는지 자세히 알 수 있는 블레이드가 열립니다. 대부분의 경우 문제를 이해하고 해결하기에 충분합니다.
3. 사용자에게 라이선스를 할당하기 전에 사용자에게 **UsageLocation** 속성이 설정되어 있는지 확인하세요. 사용자 블레이드의 **Profile** 탭을 확인하여 사용자에게 해당 속성이 설정되어 있는지 확인하세요.
4. 할당하려는 제품에 사용할 수 있는 라이선스가 충분한지 확인합니다. Azure 포털의 [Azure Active Directory -> 라이선스 -> 모든 제품 ](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products)에서 사용 가능한 라이선스 수를 확인할 수 있습니다.
5. 사용자에게 할당하려는 새 라이선스의 서비스와 충돌하는 다른 라이선스가 이미 있을 수 있습니다. 예를 들어 사용자가 Exchange 온라인(계획 1) 서비스를 사용하도록 설정한 경우 Exchange 온라인(계획 2)에서는 라이선스를 할당할 수 없습니다. 서비스 중 하나를 사용하지 않도록 설정하여 새 라이선스 할당을 허용합니다. Azure 포털 또는 PowerShell cmdlet을 사용하는 경우 **문제 세부 정보** 페이지에 충돌을 일으키는 특정 서비스가 나열됩니다.
6. 라이선스를 제거하려고 하는데 실패하는 경우 제거하려는 서비스에 종속된 서비스가 포함된 다른 라이선스가 사용자에게 있을 수 있습니다. Azure 포털 또는 PowerShell cmdlet을 사용하는 경우 종속성이 있는 특정 서비스가 오류 메시지에 나열됩니다.
7. 사용자(예: 조직의 다른 사용자가 변경했을 수 있음)로부터 라이선스를 추가/제거한 이유를 이해하려면 감사 로그를 확인하세요. 수행한 "actor"를 포함하여 모든 수정 사항을 표시하려면 필터를 **라이선스 활동** 으로 설정하세요.
8. Exchange Online을 사용하는 경우 테넌트의 일부 사용자가 동일한 프록시 주소 값으로 잘못 구성되었을 수 있습니다. 이러한 경우 라이선스 작업이 실패하면 일반 오류 메시지가 표시될 수 있습니다. [이 게시물](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used)에는 [원격 PowerShell을 사용하여 Exchange 온라인에 연결하는 방법](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)에 대한 정보를 포함하여 이 문제에 대한 자세한 정보가 포함되어 있습니다. 테넌트에서 동일한 프록시 주소를 포함하는 사용자를 식별하려면 다음 Exchange 온라인 cmdlet을 실행하세요.

실행

Get-Recipient | where {$_.EmailAddresses -match <user principal name>} | fL Name, RecipientType,emailaddresses





