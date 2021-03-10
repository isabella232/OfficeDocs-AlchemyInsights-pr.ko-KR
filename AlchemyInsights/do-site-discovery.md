---
title: 사이트 검색 시작
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529312"
---
# <a name="do-site-discovery"></a><span data-ttu-id="b3bfb-102">사이트 검색 시작</span><span class="sxs-lookup"><span data-stu-id="b3bfb-102">Do site discovery</span></span>

<span data-ttu-id="b3bfb-103">조직에서 여전히 기존 웹 응용 프로그램을 사용하고 있고 Internet Explorer 모드(대부분의 고객이 사용하는)를 사용할 계획이면 몇 가지 추가 사이트 검색을 수행해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3bfb-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="b3bfb-104">**이전 버전의 Microsoft Edge를 배포한 경우**</span><span class="sxs-lookup"><span data-stu-id="b3bfb-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="b3bfb-105">이전 버전의 Microsoft Edge에서 작동하도록 엔터프라이즈 사이트 목록을 이미 구성한 경우 사이트 검색이 거의 완료된 것입니다.</span><span class="sxs-lookup"><span data-stu-id="b3bfb-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="b3bfb-106">중립 사이트를 추가해야 할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b3bfb-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="b3bfb-107">중립 사이트는 일반적으로 SSO(Single Sign-On)를 제공하는 사이트입니다.</span><span class="sxs-lookup"><span data-stu-id="b3bfb-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="b3bfb-108">Microsoft Edge에서 중립 사이트로 이동하는 경우 Microsoft Edge에 남아 인증하려고 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3bfb-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="b3bfb-109">Internet Explorer 모드에서 중립 사이트로 이동하는 경우 Internet Explorer 모드로 유지하여 인증하려고 합니다.</span><span class="sxs-lookup"><span data-stu-id="b3bfb-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="b3bfb-110">사용하는 SSO 또는 기타 중립 사이트를 식별하여 기업 사이트 목록에 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="b3bfb-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="b3bfb-111">**Internet Explorer가 기본 브라우저로 지정된 경우**</span><span class="sxs-lookup"><span data-stu-id="b3bfb-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="b3bfb-112">Internet Explorer를 사용하고 있는 경우 최신 웹 표준으로 업그레이드한 사이트와 Internet Explorer가 여전히 필요한 사이트를 모를 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b3bfb-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="b3bfb-113">이러한 사이트에서만 Internet Explorer 모드를 사용할 수 있도록 이러한 사이트를 찾아서 기업 사이트 목록에 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b3bfb-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="b3bfb-114">[엔터프라이즈 사이트 검색](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery)은 Internet Explorer 모드가 필요할 수 있는 사이트를 검색합니다.</span><span class="sxs-lookup"><span data-stu-id="b3bfb-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="b3bfb-115">Windows 10, Windows 8.1 또는 Windows 7의 Internet Explorer 11을 통해 Windows Internet Explorer 8을 실행하는 시스템에 대한 데이터를 수집할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b3bfb-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="b3bfb-116">**데이터 분석**</span><span class="sxs-lookup"><span data-stu-id="b3bfb-116">**Analyze the data**</span></span>

<span data-ttu-id="b3bfb-117">사이트 데이터를 수집한 후에는 다음 4단계 프로세스를 통해 데이터를 분석하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="b3bfb-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="b3bfb-118">도메인별로 데이터를 정렬한 다음 URL별로 정렬합니다.</span><span class="sxs-lookup"><span data-stu-id="b3bfb-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="b3bfb-119">Internet Explorer 모드에 대해 구성할 앱의 경계를 정의합니다.</span><span class="sxs-lookup"><span data-stu-id="b3bfb-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="b3bfb-120">앱을 정의하는 모든 사이트 및 웹 컨트롤을 포함하려고 하지만 추가 사이트 및 컨트롤은 포함하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="b3bfb-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="b3bfb-121">일부 사이트는 *https://contoso.com/app1* 처럼 단순할 수 있지만 다른 사이트는 여러 사이트와 페이지를 정의해야 할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b3bfb-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="b3bfb-122">앱을 테스트하여 정상적으로 작동하지 않는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="b3bfb-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="b3bfb-123">많은 사이트에서 최신 브라우저를 검색할 때 최신 콘텐츠를 제공하고 Internet Explorer를 검색할 때만 기존 콘텐츠를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="b3bfb-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="b3bfb-124">테스트에 실패한 경우 엔터프라이즈 사이트 목록에 앱을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="b3bfb-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="b3bfb-125">앱을 구성하는 모든 사이트를 그룹화하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="b3bfb-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="b3bfb-126">이렇게 하면 앱을 업그레이드할 때 Internet Explorer 모드에서 전체 사이트를 제거하고 해당 앱에 대한 최신 브라우저를 사용하는 것이 더 쉽습니다.</span><span class="sxs-lookup"><span data-stu-id="b3bfb-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="b3bfb-127">사이트 검색을 완료하고 데이터를 분석했으면 채널 전략을 살펴볼 준비가 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="b3bfb-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>

