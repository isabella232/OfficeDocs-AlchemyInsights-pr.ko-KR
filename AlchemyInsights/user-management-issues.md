---
title: 사용자 관리 문제
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898165"
---
# <a name="user-management-issues"></a><span data-ttu-id="17d7c-102">사용자 관리 문제</span><span class="sxs-lookup"><span data-stu-id="17d7c-102">User management issues</span></span>

<span data-ttu-id="17d7c-103">**'사용자 할당 필요' 속성을 사용하지 않도록 설정하면(이 속성을 아니요로 설정) 응용 프로그램에 현재 할당된 사용자가 어떻게 되나요?**</span><span class="sxs-lookup"><span data-stu-id="17d7c-103">**What happens to current assigned users to the application if I disable the property ‘User assignment required’ (set this property to No)?**</span></span>

<span data-ttu-id="17d7c-104">**사용자 할당 필요** 를 불가능으로 설정해도 현재 할당된 사용자는 영향을 받지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="17d7c-104">Disabling **User assignment required** does NOT affect the currently assigned users.</span></span> <span data-ttu-id="17d7c-105">이 속성을 사용하지 않도록 설정하면 모든 사용자가 응용프로그램에 액세스할 수만 있습니다.</span><span class="sxs-lookup"><span data-stu-id="17d7c-105">Disabling this property will only allow all users to access the application.</span></span> <span data-ttu-id="17d7c-106">나열된 모든 사용자와 응용 프로그램에서 그룹에 할당된 사용자는 모두 유효합니다.</span><span class="sxs-lookup"><span data-stu-id="17d7c-106">All the listed users and those users assigned to groups in the application will still be valid.</span></span>

- <span data-ttu-id="17d7c-107">앱을 특정 사용자 집합으로 제한하는 경우 [Azure 애플리케이션을 사용자 집합으로 제한 - Microsoft ID 플랫폼 | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="17d7c-107">To restrict your app to specific set of users, see - [Restrict Azure AD app to a set of users - Microsoft identity platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).</span></span>
- <span data-ttu-id="17d7c-108">Azure Portal 내에서 또는 PowerShell을 사용하여 Azure AD의 엔터프라이즈 응용 프로그램에 사용자 및 그룹을 할당하려면 [Azure Active Directory의 앱에 대한 사용자 할당 관리](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="17d7c-108">To assign users and groups, to enterprise applications in Azure Active Directory (Azure AD), either from within the Azure portal or by using PowerShell, see [Manage user assignment for an app in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).</span></span>
- <span data-ttu-id="17d7c-109">응용 프로그램 만들기 및 관리 권한을 위임하려면 [응용 프로그램 관리 관리자 권한 위임 - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="17d7c-109">To delegate Application creation and management permissions, see [Delegate application management administrator permissions - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).</span></span>
- <span data-ttu-id="17d7c-110">**사용자로부터 특정 엔터프라이즈 앱 숨기기** - 다음 단계에 따라 **MyApps** 패널에서 모든 Microsoft 365 앱을 숨깁니다.</span><span class="sxs-lookup"><span data-stu-id="17d7c-110">**Hide specific enterprise apps from users** - Use the following steps to hide all Microsoft 365 apps from the **MyApps** panel.</span></span> <span data-ttu-id="17d7c-111">Office 365 포털에도 앱이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="17d7c-111">The apps will still be visible in the Office 365 portal.</span></span>

 1. <span data-ttu-id="17d7c-112">디렉터리의 전역 관리자로 Azure Portal에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="17d7c-112">Sign-in to the Azure portal as a global administrator for your directory.</span></span> 
 2. <span data-ttu-id="17d7c-113">**Azure Active Directory** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="17d7c-113">Select **Azure Active Directory**.</span></span> 
 3. <span data-ttu-id="17d7c-114">**사용자** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="17d7c-114">Select **Users**.</span></span> 
 4. <span data-ttu-id="17d7c-115">**사용자 설정** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="17d7c-115">Select **User settings**.</span></span> 
 5. <span data-ttu-id="17d7c-116">**엔터프라이즈 응용 프로그램** 에서 **최종 사용자 실행 및 응용 프로그램 보기 관리** 를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="17d7c-116">Under **Enterprise applications**, click **Manage how end users launch and view their applications**.</span></span> 
 6. <span data-ttu-id="17d7c-117">**Office 365 포털의 사용자만 Office 365 앱을 볼 수 있음** 에 대해 **예** 를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="17d7c-117">For **Users can only see Office 365 apps in the Office 365 portal**, click **Yes**.</span></span> 
 7. <span data-ttu-id="17d7c-118">**저장** 을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="17d7c-118">Click **Save**.</span></span> 
 8. <span data-ttu-id="17d7c-119">자세한 내용은 [Microsoft Azure AD의 사용자 환경에서 터프라이즈 응용 프로그램 숨기기 | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="17d7c-119">For more details, see [Hide an Enterprise application from user's experience in Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)</span></span>

- <span data-ttu-id="17d7c-120">SaaS(Software as a Service) 앱을 여러 조직에 제공하는 경우 Azure AD(Azure Active Directory) 테넌트에서 로그인을 수락하도록 앱을 구성할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="17d7c-120">If you offer a Software as a Service (SaaS) app to many organizations, you can configure your app to accept sign-ins from any Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="17d7c-121">이 구성을 "응용 프로그램 다중 테넌트 만들기"라고 합니다.</span><span class="sxs-lookup"><span data-stu-id="17d7c-121">This configuration is called "making your application multi-tenant".</span></span> <span data-ttu-id="17d7c-122">Azure AD 테넌트의 사용자는 앱에 계정을 사용하는 데 동의한 후 앱에 로그인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="17d7c-122">Users in any Azure AD tenant will be able to sign-in to your app after consenting to use their account with your app.</span></span> <span data-ttu-id="17d7c-123">자세한 내용은 [Azure AD 사용자에 로그인하는 앱 빌드 - Microsoft ID 플랫폼 | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="17d7c-123">For more information, see [Build apps that sign in Azure AD users - Microsoft identity platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).</span></span>

- <span data-ttu-id="17d7c-124">**최종 사용자가 응용 프로그램에 할당된 후 응용 프로그램에 어떻게 액세스할 수 있나요?**</span><span class="sxs-lookup"><span data-stu-id="17d7c-124">**How can an end user access the application once he/she is assigned to the application?**</span></span>

<span data-ttu-id="17d7c-125">엔터프라이즈 응용 프로그램의 각 응용 프로그램에는 최종 사용자가 액세스할 수 있는 링크가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="17d7c-125">Each app in Enterprise application blade has a link for end users to access.</span></span> <span data-ttu-id="17d7c-126">사용자는 **Myapps** 포털을 통해 앱에 쉽게 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="17d7c-126">Users can also access the app through **Myapps** portal in an easy way.</span></span>

- <span data-ttu-id="17d7c-127">**사용자가 사용하려는 응용 프로그램과 응용 프로그램 유형을 알고 싶나요?**</span><span class="sxs-lookup"><span data-stu-id="17d7c-127">**Want to know which applications and type of applications are being used by users?**</span></span>

<span data-ttu-id="17d7c-128">**portal.azure.com > Azure Active directory> 로그인> 보고서 다운로드** 에서 지난 30일간의 로그인 보고서를 다운로드할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="17d7c-128">You can download sign-in reports for the last 30 days from **portal.azure.com > Azure Active directory> Signins> download reports**.</span></span>

- <span data-ttu-id="17d7c-129">[테넌트 전체 관리자에게 응용 프로그램에 대한 동의 허용](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) 및 [최종 사용자가 응용 프로그램에 동의하는 방식을 구성하는 방법](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent)에 대해 알아봅니다.</span><span class="sxs-lookup"><span data-stu-id="17d7c-129">Learn how to [Grant tenant wide admin consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) and [Configure how end users consent to applications](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).</span></span>

- <span data-ttu-id="17d7c-130">[동의 작동 방식](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 및 [응용 프로그램에 대한 동의 관리](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests)를 이해합니다.</span><span class="sxs-lookup"><span data-stu-id="17d7c-130">Understand [how consent works](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) and [Manage consent to applications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).</span></span>


