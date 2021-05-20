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
# <a name="create-user"></a><span data-ttu-id="61f12-102">Create user(사용자 만들기)</span><span class="sxs-lookup"><span data-stu-id="61f12-102">Create user</span></span>

<span data-ttu-id="61f12-103">**공지 사항:**</span><span class="sxs-lookup"><span data-stu-id="61f12-103">**ANNOUNCEMENT:**</span></span>

- <span data-ttu-id="61f12-104">[2021년 1월 4일부터 Google에서 WebView](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) 로그인 지원 사용이 더 이상 사용 안 됩니다.</span><span class="sxs-lookup"><span data-stu-id="61f12-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) .</span></span> <span data-ttu-id="61f12-105">호환성 테스트에 대한 [Google의](https://go.microsoft.com/fwlink/?linkid=2157323) 지침을 따라 앱이 영향을 받을 수 있는지 테스트합니다.</span><span class="sxs-lookup"><span data-stu-id="61f12-105">Test whether your apps may be affected by following [Google’s guidance](https://go.microsoft.com/fwlink/?linkid=2157323) on testing compatibility.</span></span>
- <span data-ttu-id="61f12-106">소비자 Google 계정을 사용하여 사용자에 로그인할 때 시스템 웹 보기 또는 시스템 브라우저를 사용하는지 확인</span><span class="sxs-lookup"><span data-stu-id="61f12-106">Make sure you use the system webview or system browser when signing in your users with consumer Google accounts.</span></span> <span data-ttu-id="61f12-107">자세한 내용은 [Chrome 브라우저만 사용하여 응용 프로그램에 로그인하는 문제](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="61f12-107">For more information, see [Issues signing in to application(s) using Chrome browser only](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span></span>

<span data-ttu-id="61f12-108">**Azure AD 디렉터리에서 새 사용자를 생성할 수 없습니다.**</span><span class="sxs-lookup"><span data-stu-id="61f12-108">**I can't create a new user in my Azure AD directory**</span></span>

1. <span data-ttu-id="61f12-109">새 표준 사용자를 생성할 권한이 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="61f12-109">Ensure that you are authorized to create a new standard user.</span></span> <span data-ttu-id="61f12-110">AD(Azure Active Directory)의 전역 관리자 또는 사용자 관리자 역할만 새 표준 사용자를 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="61f12-110">Only the Global administrator or User administrator role in Azure Active Directory (AD) can create a new standard user.</span></span> <span data-ttu-id="61f12-111">이러한 역할 중 하나가 아닌 경우 관리자에게 이러한 역할 중 하나에 사용자를 추가하거나 새 사용자 계정을 만들도록 요청하세요.</span><span class="sxs-lookup"><span data-stu-id="61f12-111">If you're not in one of these roles, ask an administrator to add you to one of these roles or to create the new user account for you.</span></span>
1. <span data-ttu-id="61f12-112">사용자 이름이 Azure AD에서 확인된 도메인에 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="61f12-112">Ensure that the user name is in a domain that is verified in your Azure AD.</span></span> <span data-ttu-id="61f12-113">Azure AD에 확인된 사용자 지정 도메인 이름이 없는 경우 \*.onmicrosoft.com으로 끝나는 Azure AD 초기 도메인을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="61f12-113">If you do not have any verified custom domain names in your Azure AD, you can use your Azure AD initial domain, which ends with \*.onmicrosoft.com.</span></span>
1. <span data-ttu-id="61f12-114">사용자 이름이 온-프레미스 AD에서 Azure AD로 연합되지 않은 도메인에 있는지 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="61f12-114">Ensure that the user name is in a domain that is not federated to Azure AD from your on-premises AD.</span></span> <span data-ttu-id="61f12-115">사내에서 연합된 도메인 이름으로 사용자를 클라우드에 추가할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="61f12-115">Users cannot be added in the cloud with domain names that are federated from on-premises.</span></span>
1. <span data-ttu-id="61f12-116">새 사용자에게 할당할 사용자 이름을 이미 가지고 있는 다른 사용자 또는 연락처가 없는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="61f12-116">Ensure that no other user or contact already has the user name that you want to assign to the new user.</span></span> <span data-ttu-id="61f12-117">사용자 이름은 Azure AD 전반에서 고유해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="61f12-117">User names must be unique across Azure AD.</span></span>
1. <span data-ttu-id="61f12-118">Azure AD의 경우 [Azure AD 역할 및 관리자](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="61f12-118">See [Azure AD roles and administrators](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="61f12-119">Azure AD의 경우 [도메인 이름](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="61f12-119">See the [domain names](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="61f12-120">[감사 로그 ](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators)을(를) 검토하여 작업을 수행한 사용자와 같이 최근에 생성되거나 삭제된 사용자에 대한 자세한 정보를 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="61f12-120">Review [Audit logs](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) to see more detailed information about a recently created or deleted user like who performed the action and when.</span></span>
1. <span data-ttu-id="61f12-121">새 사용자를 추가하는 데 대한 자세한 내용은 Azure Portal을 사용하여 Azure AD에서 새 사용자 [만들기를 참조하세요.](/azure/active-directory/active-directory-users-create-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="61f12-121">For more information on adding new users, see [Use the Azure portal to create a new user in your Azure AD](/azure/active-directory/active-directory-users-create-azure-portal).</span></span>
1. <span data-ttu-id="61f12-122">[Azure AD 관리 역할:](/azure/active-directory/active-directory-assign-admin-roles)Azure의 관리자 역할 Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="61f12-122">[Azure AD administrative roles](/azure/active-directory/active-directory-assign-admin-roles): Administrator role permissions in Azure Active Directory</span></span>
1. <span data-ttu-id="61f12-123">Azure [AD PowerShell을](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)사용하여 새 사용자를 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="61f12-123">You can also [use Azure AD PowerShell to create a new user](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).</span></span>
