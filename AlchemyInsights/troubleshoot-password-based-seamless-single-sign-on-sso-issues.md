---
title: 암호 기반 원활한 SSO(Single Sign-On) 문제 해결
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709498"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a><span data-ttu-id="43511-102">암호 기반 원활한 SSO(Single Sign-On) 문제 해결</span><span class="sxs-lookup"><span data-stu-id="43511-102">Troubleshoot Password-based Seamless Single Sign-on (SSO) issues</span></span>

<span data-ttu-id="43511-103">암호 기반 SSO의 기본에 대한 자세한 내용은 Azure Active Directory를 사용하는 암호 기반 [인증을 참조하세요.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="43511-103">To learn the fundamentals of password-based SSO, see [Password-based authentication with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span></span>

<span data-ttu-id="43511-104">**암호 기반 SSO 구성**</span><span class="sxs-lookup"><span data-stu-id="43511-104">**Configure Password-based SSO**</span></span>

1. <span data-ttu-id="43511-105">[암호 기반 Single Sign-On](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) 구성 - 이 문서에서는 암호 기반 SSO 옵션에 대해 자세히 설명하고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="43511-105">[Configure password-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - This article goes into more detail about the password-based SSO option.</span></span> <span data-ttu-id="43511-106">추가할 응용 프로그램에 사용자 지정 구성이 필요하고 암호 기반 SSO를 사용해야 하는 경우 이 문서가 도움이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="43511-106">If the application you're adding requires custom configuration and you need to use password-based SSO, then this article is for you.</span></span>
2. <span data-ttu-id="43511-107">[프레미스 앱에](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) 대한 암호 기반 Single Sign-On 구성 - 응용 프로그램 프록시는 몇 가지 Single Sign-On 모드를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="43511-107">[Configure password-based single sign on for on-prem apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Application Proxy supports several single sign-on modes.</span></span> <span data-ttu-id="43511-108">암호 기반 로그인은 인증에 사용자 이름/암호 조합을 사용하는 응용 프로그램을 위한 것입니다.</span><span class="sxs-lookup"><span data-stu-id="43511-108">Password-based sign-on is intended for applications that use a username/password combination for authentication.</span></span> <span data-ttu-id="43511-109">응용 프로그램에 대해 암호 기반 로그인을 구성할 때 사용자는 한 번만 On-premises 응용 프로그램에 로그인해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="43511-109">When you configure password-based sign-on for your application, your users have to sign in to the on-premises application once.</span></span> <span data-ttu-id="43511-110">그런 다음 Azure Active Directory는 로그인 정보를 저장하고 사용자가 원격으로 액세스할 때 응용 프로그램에 자동으로 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="43511-110">After that, Azure Active Directory stores the sign-in information and automatically provides it to the application when your users access it remotely.</span></span>
    - <span data-ttu-id="43511-111">응용 프로그램 프록시를 사용하여 앱을 게시하고 테스트해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="43511-111">You should already have published and tested your app with Application Proxy.</span></span> <span data-ttu-id="43511-112">그렇지 않은 경우 [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) 응용 프로그램 프록시를 사용하여 응용 프로그램 게시의 단계를 따라 프레미스 앱에 대한 암호 기반 SSO 구성을 계속합니다.</span><span class="sxs-lookup"><span data-stu-id="43511-112">If not, follow the steps in [Publish applications using Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) then continue your configuration of password-based SSO for on-prem apps.</span></span>

<span data-ttu-id="43511-113">암호 기반 SSO 문제 해결을 위해 Azure AD에서 암호 기반 [Single Sign-On 문제 해결을 참조하세요.](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="43511-113">To troubleshoot password-based SSO, see [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span></span>
