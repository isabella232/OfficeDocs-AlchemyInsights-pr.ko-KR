---
title: 링크 및 URL 문제
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: f682afc2006957a83d02973d28e2a07ee63ac888
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707888"
---
# <a name="issues-with-links-and-urls"></a><span data-ttu-id="2d5ed-102">링크 및 URL 문제</span><span class="sxs-lookup"><span data-stu-id="2d5ed-102">Issues with links and URLs</span></span>

<span data-ttu-id="2d5ed-103">리디렉션 URI/회신 URL(두 표현은 모두 교환 가능)은 Microsoft ID 플랫폼에서 앱 요청 토큰을 반환하는 데 사용되는 URL입니다.</span><span class="sxs-lookup"><span data-stu-id="2d5ed-103">Redirect URI/reply URLs (both expressions are interchangeable) are the URLs used by the Microsoft identity platform to return app-requested tokens.</span></span> <span data-ttu-id="2d5ed-104">이 URL에 대한 내용은 다음 문서를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="2d5ed-104">For information on these URLs, see the following articles:</span></span>

- <span data-ttu-id="2d5ed-105">[인증 흐름 및 응용 프로그램 시나리오](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - 각 시나리오에 대한 **앱 등록** 페이지의 리디렉션 URI에 대한 정보입니다.</span><span class="sxs-lookup"><span data-stu-id="2d5ed-105">[Authentication flows and application scenarios](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - Information about the redirect URIs in the **App registration** page for each scenario.</span></span>
- [<span data-ttu-id="2d5ed-106">리디렉션 URI/회신 URL 제한사항 및 한계</span><span class="sxs-lookup"><span data-stu-id="2d5ed-106">Redirect URI/reply URL restrictions and limitations</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

<span data-ttu-id="2d5ed-107">**앱에 대한 올바른 리디렉션 URI/회신 URL을 등록하는 방법을 모르는 경우**</span><span class="sxs-lookup"><span data-stu-id="2d5ed-107">**I don't know how to register the right redirect URI / reply URL for my app**</span></span>

<span data-ttu-id="2d5ed-108">개발 중인 응용 프로그램으로 로그인할 때 로그인 대화 상자에 **AADS50011이 표시되는 경우: 요청에 지정된 응답 URL이 응용 프로그램 <your app ID>** 에 대해 구성된 응답 URL과 일치하지 않습니다. 응용 프로그램 등록에 코드를 사용하여 Microsoft ID 플랫폼에 요청한 리디렉션 URI를 추가해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d5ed-108">When you sign in with the application you are developing, if the sign-in dialog displays **AADSTS50011: The reply url specified in the request does not match the reply urls configured for the application <your app ID>**, you'll need to add to your application registration, the redirect URI that your code used in the token request to the Microsoft identity platform.</span></span>

<span data-ttu-id="2d5ed-109">회신 URL을 추가하기 위해 Azure Portal의 **응용 프로그램 등록** 페이지에서 **인증** 탭으로 이동한 다음 **리디렉션 URI** 섹션에 항목을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="2d5ed-109">To add a reply URL, go to the **Authentication** tab in your **application registration** page in the Azure portal and add an entry in the **Redirect URIs** section.</span></span> <span data-ttu-id="2d5ed-110">입력해야 하는 값은 아래 설명된 바와 같이 구축하는 응용 프로그램의 유형에 따라 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="2d5ed-110">The value you need to enter depends on the type of application you're building, as described below:</span></span>

- <span data-ttu-id="2d5ed-111">단일 페이지 응용 프로그램 및 웹앱의 경우 회신 URL은 응용 프로그램의 URL입니다.</span><span class="sxs-lookup"><span data-stu-id="2d5ed-111">For single-page applications and web apps, the reply URL is a URL in your application.</span></span> <span data-ttu-id="2d5ed-112">[단일 페이지 응용 프로그램 등록](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) 또는 [Azure Portal을 사용하여 웹 응용 프로그램 등록](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)을 참조하십시오.</span><span class="sxs-lookup"><span data-stu-id="2d5ed-112">See [Single-page application registration](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) or [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)</span></span>
- <span data-ttu-id="2d5ed-113">데스크톱 앱의 경우 선택해야 하는 값은 다음에 따라 선택해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="2d5ed-113">For desktop apps, the value that you need to choose depends on:</span></span>
    - <span data-ttu-id="2d5ed-114">플랫폼(MacOS는 Windows 또는 버전과 다를 수 있습니다.)</span><span class="sxs-lookup"><span data-stu-id="2d5ed-114">the platform (MacOS is different from Windows or Linux)</span></span>
    - <span data-ttu-id="2d5ed-115">통합 Windows 인증 [IWA] 또는 사용자 이름/암호를 사용하여 장치 코드 흐름을 통해 대화형 토큰을 획득하는 방식입니다.</span><span class="sxs-lookup"><span data-stu-id="2d5ed-115">the way you acquire the token (interactively, with device code flow, with Integrated Windows Authentication [IWA] or with username/password).</span></span>
    <span data-ttu-id="2d5ed-116">자세한 내용은 [데스크톱 앱 - 앱 등록 - 리디렉션 URi를 참조하세요.](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)</span><span class="sxs-lookup"><span data-stu-id="2d5ed-116">For details, see [Desktop apps - App registration - Redirect URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)</span></span>
- <span data-ttu-id="2d5ed-117">모바일 응용 프로그램의 경우 리디렉션 URI는 다음에 따라 다를 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d5ed-117">For mobile applications, the redirect URI depends on:</span></span>
    - <span data-ttu-id="2d5ed-118">플랫폼(iOS/Android/UWP)</span><span class="sxs-lookup"><span data-stu-id="2d5ed-118">the platform (iOS/Android/UWP)</span></span>
    - <span data-ttu-id="2d5ed-119">iOS의 번들 ID와 같은 앱을 빌드하는 데 사용되는 정보와 Android Azure Portal 앱 등록의 패키지 이름 및 서명 해시가 도움이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="2d5ed-119">the information used to build your app, such as the bundle ID in iOS, and the package name and signature hash on Android The Azure portal app registration will help you.</span></span> <span data-ttu-id="2d5ed-120">자세한 내용은 [플랫폼 구성 및 리디렉션 URI](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="2d5ed-120">For details, see [Platform configuration and redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).</span></span>

> [!NOTE]
> <span data-ttu-id="2d5ed-121">웹 API 및 IWA(사용자 이름/암호)를 자동으로 사용하는 일부 방법은 리디렉션 URI가 필요하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="2d5ed-121">Web APIs and some of the silent ways of acquiring tokens (IWA and username/password) don't require a redirect URI.</span></span>

<span data-ttu-id="2d5ed-122">**웹 응용 프로그램을 배포했습니다. 배포된 앱을 테스트할 때 회신 URL 불일치 메시지가 나타나는 경우**</span><span class="sxs-lookup"><span data-stu-id="2d5ed-122">**I've deployed my web application and when I test the deployed app, I get a reply url mismatch message**</span></span>

<span data-ttu-id="2d5ed-123">웹 응용 프로그램을 배포하는 모든 위치에 대한 리디렉션 URI를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="2d5ed-123">Add redirect URIs for all the locations at which you are deploying your web application.</span></span> <span data-ttu-id="2d5ed-124">자세한 내용은 [Azure Portal을 사용하여 웹앱 앱 등록](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="2d5ed-124">For more information, see [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).</span></span>

> [!NOTE]
> <span data-ttu-id="2d5ed-125">해당 위치에 응용 프로그램을 배포한 직후 위치에 대한 리디렉션 URI를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="2d5ed-125">Add redirect URI for a location immediately after you have deployed the application at that location.</span></span>

<span data-ttu-id="2d5ed-126">**충분한 회신 URL을 등록할 수 없는 경우**</span><span class="sxs-lookup"><span data-stu-id="2d5ed-126">**I can't register enough reply URLs**</span></span>

<span data-ttu-id="2d5ed-127">ISV인 경우 모든 고객에 대해 하나 또는 여러 개의 리디렉션 URI가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2d5ed-127">You're an ISV and have one or several redirect URIs for every customer of yours.</span></span> <span data-ttu-id="2d5ed-128">ADAL/Azure AD v1.0에서 MSAL/Microsoft ID 플랫폼으로 마이그레이션하려는 경우 [리디렉션 URI의 최대 개수](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris)에 도달합니다.</span><span class="sxs-lookup"><span data-stu-id="2d5ed-128">You want to migrate from ADAL/Azure AD v1.0 to MSAL/the Microsoft identity platform and you hit the [maximum number of redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris).</span></span> <span data-ttu-id="2d5ed-129">이 문제를 해결하기 위해 [해당하는 서비스에 리디렉션 URI를 추가](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals)합니다.</span><span class="sxs-lookup"><span data-stu-id="2d5ed-129">To resolve this, [add redirect URIs to service principals](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) that correspond to each of your customers.</span></span>
