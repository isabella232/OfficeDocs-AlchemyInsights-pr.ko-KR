---
title: SharePoint의 Yammer 웹 파트
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5475"
- "9002494"
ms.openlocfilehash: d8b4043bb2889429a18c477505e7eca662943051
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664356"
---
# <a name="yammer-web-parts-in-sharepoint"></a><span data-ttu-id="c89d3-102">SharePoint의 Yammer 웹 파트</span><span class="sxs-lookup"><span data-stu-id="c89d3-102">Yammer web parts in SharePoint</span></span>

<span data-ttu-id="c89d3-103">Yammer 대화 및 Yammer 하이라이트 웹 파트는 최신 및 클래식 SharePoint 페이지에서 공동 작업을 향상시킵니다.</span><span class="sxs-lookup"><span data-stu-id="c89d3-103">Yammer Conversations and Yammer Highlights web parts enhance collaboration on modern and classic SharePoint pages.</span></span> <span data-ttu-id="c89d3-104">자세한 내용은 [Yammer 대화](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#conversations) 및 [Yammer 하이라이트](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#highlights)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c89d3-104">For more info, see [Yammer Conversations](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#conversations)  and  [Yammer Highlights](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da#highlights).</span></span>    

<span data-ttu-id="c89d3-105">최신 Yammer 대화 웹 파트는 새 Yammer 환경으로 업데이트되며 대상 릴리스 테넌트가 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c89d3-105">The modern Yammer Conversations web part is being updated to the new Yammer experience and is available for Targeted Release tenants.</span></span> <span data-ttu-id="c89d3-106">GA 롤아웃을 시작했습니다.</span><span class="sxs-lookup"><span data-stu-id="c89d3-106">GA rollout has started.</span></span> <span data-ttu-id="c89d3-107">새로운 기능에는 모든 게시물(질문, 설문, 칭찬)과 대화를 시작하고 SharePoint에서 직접 최적의 답변을 표시하는 기능이 포함되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c89d3-107">New features include the ability to start a conversation with any post (Questions, Polls, Praise) and to mark best answers directly from SharePoint.</span></span> <span data-ttu-id="c89d3-108">자세한 내용은 [새 Yammer 고객 약관 및 FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/newyammer-faq)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c89d3-108">For more info, see [New Yammer customer terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/newyammer-faq).</span></span>

 <span data-ttu-id="c89d3-109">사용자에게 적합한 웹 파트 및 구성을 이해하려면 [SharePoint Online에서 Yammer 웹 파트 사용](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c89d3-109">To understand which web part and configuration is right for you, see [Use a Yammer web part in SharePoint Online](https://support.microsoft.com/office/use-a-yammer-web-part-in-sharepoint-online-a53cfa0c-3d09-42c8-a286-1038a81c59da).</span></span>  

<span data-ttu-id="c89d3-110">**SharePoint Server에서 웹 파트 사용하기**</span><span class="sxs-lookup"><span data-stu-id="c89d3-110">**Using web parts with SharePoint Server**</span></span>  

<span data-ttu-id="c89d3-111">웹 파트는 온-프레미스 환경 내의 최신 페이지 및 클래식 페이지에서 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c89d3-111">Web parts can be used in modern and classic pages within on-premises environments.</span></span>

- <span data-ttu-id="c89d3-112">최신 페이지에 대한 자세한 내용은 [SharePoint Server 2019의 최신 페이지에 Yammer 피드 추가](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-modern-page-in-sharepoint-server-2019)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c89d3-112">For more info about modern pages, see [Add a Yammer feed to a modern page in SharePoint Server 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-modern-page-in-sharepoint-server-2019).</span></span> 
- <span data-ttu-id="c89d3-113">클래식 페이지에 대한 자세한 내용은 [SharePoint Server 2013, 2016 및 2019의 클래식 페이지에 Yammer 피드 추가](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-classic-page-in-sharepoint-servers-2013-2016-and-2019)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c89d3-113">For more info about classic pages, see [Add a Yammer feed to a classic page in SharePoint Servers 2013, 2016, and 2019](https://docs.microsoft.com/yammer/integrate-yammer-with-other-apps/embed-a-feed-into-a-sharepoint-site#add-a-yammer-feed-to-a-classic-page-in-sharepoint-servers-2013-2016-and-2019).</span></span>

<span data-ttu-id="c89d3-114">**Yammer 임베드**</span><span class="sxs-lookup"><span data-stu-id="c89d3-114">**Yammer Embed**</span></span>  

<span data-ttu-id="c89d3-115">임베드 구성 도구를 사용하여 임베드 사용을 테스트합니다.</span><span class="sxs-lookup"><span data-stu-id="c89d3-115">Use the Embed Configuration tool to test Embed usage.</span></span> <span data-ttu-id="c89d3-116">임베드 추후 업데이트를 통해 새 Yammer 환경을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c89d3-116">A future update to Embed will enable the new Yammer experience.</span></span> <span data-ttu-id="c89d3-117">자세한 내용은 [Yammer 임베드 구성 도구](https://aka.ms/YammerEmbedConfigureTool)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c89d3-117">For more info, see the [Yammer Embed Configuration tool](https://aka.ms/YammerEmbedConfigureTool).</span></span> <span data-ttu-id="c89d3-118">Yammer 임베드 구성 요소를 보다 잘 이해하려면 [임베드 피드](https://aka.ms/YammerDevDocs)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c89d3-118">To better understand the Yammer Embed component, see [Embed Feed](https://aka.ms/YammerDevDocs).</span></span>

<span data-ttu-id="c89d3-119">**알려진 문제점 및 제한 사항**</span><span class="sxs-lookup"><span data-stu-id="c89d3-119">**Known issues and limitations**</span></span>

- <span data-ttu-id="c89d3-120">그룹 ID는 변경된 새 Yammer URL에서 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="c89d3-120">Group IDs are not available from new Yammer URLs, which have changed.</span></span> <span data-ttu-id="c89d3-121">클래식 모드로 다시 전환하여 URL에서 그룹 ID 또는 다른 ID를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="c89d3-121">Switch back to classic mode to obtain group IDs or other IDs from URLs.</span></span>
- <span data-ttu-id="c89d3-122">사용자 지정(베니티) 도메인은 지원되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="c89d3-122">Custom (vanity) domains are not supported.</span></span>
- <span data-ttu-id="c89d3-123">Yammer 임베드는 모바일에 최적화되지 않았습니다.</span><span class="sxs-lookup"><span data-stu-id="c89d3-123">Yammer Embed is not optimized for mobile.</span></span> <span data-ttu-id="c89d3-124">최적의 환경을 위해 Yammer 대화 웹 파트를 사용하여 최신 페이지를 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="c89d3-124">Use modern pages with the Yammer Conversations web part for the best experience.</span></span>
- <span data-ttu-id="c89d3-125">사용자 지정 테마는 Yammer 대화 웹 파트의 모양과 사용 편리성에 영향을 줄 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c89d3-125">Custom themes can affect the appearance and usability of the Yammer Conversations web part.</span></span> <span data-ttu-id="c89d3-126">지원 사례를 열면 문제를 보고할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c89d3-126">Open a support case to report issues.</span></span>