---
title: 원활한 SSO 사용자 로그인 문제
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
- "9004357"
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/21/2021
ms.locfileid: "49919204"
---
# <a name="seamless-sso-user-sign-in-issues"></a><span data-ttu-id="9cc10-102">원활한 SSO 사용자 로그인 문제</span><span class="sxs-lookup"><span data-stu-id="9cc10-102">Seamless SSO user sign-in issues</span></span>

<span data-ttu-id="9cc10-103">사용자가 인증된 후 브라우저는 사용자의 자격 증명을 캐시하여 동일한 브라우저에서 응용 프로그램이 동일한 계정으로 자동으로 로그인하도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="9cc10-103">After the user is authenticated, the browser will cache the user's credentials, so that on the same browser, the application will automatically sign-in with the same account.</span></span> <span data-ttu-id="9cc10-104">이렇게 하여 다른 사용자나 한 사용자가 한 장치에서 여러 계정에 로그인하기 어려울 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9cc10-104">This may make it difficult for another user or a single user to log into multiple accounts on one device.</span></span> <span data-ttu-id="9cc10-105">이 문제를 해결하기 위해 1.</span><span class="sxs-lookup"><span data-stu-id="9cc10-105">To solve this: 1.</span></span> <span data-ttu-id="9cc10-106">다른 브라우저에서 로그인해 보십시오.</span><span class="sxs-lookup"><span data-stu-id="9cc10-106">Try signing in on another browser.</span></span> <span data-ttu-id="9cc10-107">2.</span><span class="sxs-lookup"><span data-stu-id="9cc10-107">2.</span></span> <span data-ttu-id="9cc10-108">브라우저의 캐시 및/또는 쿠키를 지우고 다시 로그인을 시도합니다.</span><span class="sxs-lookup"><span data-stu-id="9cc10-108">Clear the browser's cache and/or cookies and try signing in again.</span></span>

<span data-ttu-id="9cc10-109">여전히 로그인 문제가 발생하는 경우 다음을 수행하여 해결 단계를 진단하고 자동화하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="9cc10-109">If you are still experiencing sign-in issues, we recommend the following to diagnose and automate the resolution steps:</span></span>

1. <span data-ttu-id="9cc10-110">내 앱 보안 [브라우저 확장을](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) 설치하여 Azure AD(Azure Active Directory)가 Azure Portal에서 테스트 환경을 사용할 때 더 나은 진단 및 해결 방법을 제공할 수 있도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="9cc10-110">Install the [My Apps Secure Browser Extension](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) to help Azure Active Directory (Azure AD) to provide better diagnosis and resolutions when using the testing experience in the Azure portal.</span></span>
2. <span data-ttu-id="9cc10-111">Azure Portal의 앱 구성 페이지에서 테스트 환경을 사용하여 오류를 재현합니다.</span><span class="sxs-lookup"><span data-stu-id="9cc10-111">Reproduce the error using the testing experience in the app configuration page in the Azure portal.</span></span> <span data-ttu-id="9cc10-112">자세한 내용은 SAML 기반 Single Sign-On 응용 프로그램 디버그를 [참조합니다.](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues)</span><span class="sxs-lookup"><span data-stu-id="9cc10-112">To learn more, see [Debug SAML-based single sign-on applications](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues).</span></span>
3. <span data-ttu-id="9cc10-113">Azure Portal의 테스트 환경을 내 앱 보안 브라우저 확장과 함께 사용하는 경우 **4단계를 건너뛸 수 있습니다.**</span><span class="sxs-lookup"><span data-stu-id="9cc10-113">If you use the testing experience in the Azure portal with the My Apps Secure Browser Extension, you can **skip step 4**.</span></span>
4. <span data-ttu-id="9cc10-114">SAML 기반 Single Sign-On 구성 페이지를 열하려면</span><span class="sxs-lookup"><span data-stu-id="9cc10-114">To open the SAML-based single sign-on configuration page:</span></span>
    - <span data-ttu-id="9cc10-115">Azure [Portal을](https://portal.azure.com/) 열고 전역  관리자 또는 **Coadmin으로 로그인합니다.**</span><span class="sxs-lookup"><span data-stu-id="9cc10-115">Open the [Azure portal](https://portal.azure.com/) and sign in as a **Global Administrator** or **Coadmin**.</span></span>
    - <span data-ttu-id="9cc10-116">왼쪽 주 탐색 메뉴의  맨 위에 있는 모든 서비스를 선택하여 **Azure Active Directory** 확장을 열 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9cc10-116">Open the **Azure Active Directory Extension** by selecting **All services** at the top of the main left-side navigation menu.</span></span>
    - <span data-ttu-id="9cc10-117">필터 검색 상자에 "Azure Active Directory"를 입력하고 **Azure Active Directory 항목을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="9cc10-117">Type "Azure Active Directory" in the filter search box and select the **Azure Active Directory** item.</span></span>
    - <span data-ttu-id="9cc10-118">Azure **Active** Directory 왼쪽 탐색 메뉴에서 엔터프라이즈 응용 프로그램을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="9cc10-118">Select **Enterprise Applications** from the Azure Active Directory left-hand navigation menu.</span></span>
    - <span data-ttu-id="9cc10-119">모든 **응용 프로그램을 선택하여** 모든 응용 프로그램 목록을 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9cc10-119">Select **All Applications** to view a list of all your applications.</span></span> <span data-ttu-id="9cc10-120">여기에 표시하려는 응용 프로그램이 없는 경우 모든  응용 프로그램 목록의  맨 위에 있는 필터 컨트롤을 사용하여 표시 **옵션을** 모든 응용 프로그램으로 **설정하십시오.**</span><span class="sxs-lookup"><span data-stu-id="9cc10-120">If you do not see the application you want show up here, use the **Filter** control at the top of the **All Applications List** and set the **Show** option to **All Applications**.</span></span>
    - <span data-ttu-id="9cc10-121">Single Sign-On에 대해 구성할 응용 프로그램을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="9cc10-121">Select the application you want to configure for single sign-on.</span></span>
    - <span data-ttu-id="9cc10-122">응용 프로그램이 로드된 후 응용 프로그램의 왼쪽 탐색 메뉴에서 **Single Sign-On을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="9cc10-122">After the application loads, select **Single sign-on** from the application’s left-hand navigation menu.</span></span>
    - <span data-ttu-id="9cc10-123">**SAML 기반 SSO를 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="9cc10-123">Select **SAML-based SSO**.</span></span>
5. <span data-ttu-id="9cc10-124">오류에 따라 따라야 하는 권장 단계에 대한 자세한 내용은 SAML 기반 Single Sign-On 구성된 앱에 로그인하는 데 문제가 있는 경우를 [참조하세요.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory)</span><span class="sxs-lookup"><span data-stu-id="9cc10-124">Based on the error, to learn more about the recommended steps to follow, see [Problems signing in to SAML-based single sign-on configured apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory).</span></span>
6. <span data-ttu-id="9cc10-125">다른 사용자 서명 문제를 해결하기 위해 다음 지침을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="9cc10-125">To troubleshoot other user sign-issues refer to the following guidance:</span></span>
    - [<span data-ttu-id="9cc10-126">단일 Sign-On SAML 프로토콜</span><span class="sxs-lookup"><span data-stu-id="9cc10-126">Single Sign-On SAML protocol</span></span>](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [<span data-ttu-id="9cc10-127">방법: Azure Active Directory 보고서를 사용하여 로그인 오류 해결</span><span class="sxs-lookup"><span data-stu-id="9cc10-127">How to: Troubleshoot sign-in errors using Azure Active Directory reports</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [<span data-ttu-id="9cc10-128">예기치 않은 동의 프롬프트</span><span class="sxs-lookup"><span data-stu-id="9cc10-128">Unexpected consent prompt</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [<span data-ttu-id="9cc10-129">사용자 동의 오류</span><span class="sxs-lookup"><span data-stu-id="9cc10-129">User consent error</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [<span data-ttu-id="9cc10-130">내 앱에서 로그인하는 데 문제가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9cc10-130">Problems signing in from My Apps</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [<span data-ttu-id="9cc10-131">응용 프로그램 로그인 페이지의 오류</span><span class="sxs-lookup"><span data-stu-id="9cc10-131">Error on application sign-in page</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [<span data-ttu-id="9cc10-132">Microsoft 앱에 로그인하는 데 문제가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9cc10-132">Problem signing into a Microsoft App</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
