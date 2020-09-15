---
title: 콘텐츠가 SharePoint 검색 결과에 표시 되지 않음
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713136"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="f1e33-102">콘텐츠가 SharePoint 검색 결과에 표시 되지 않음</span><span class="sxs-lookup"><span data-stu-id="f1e33-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="f1e33-103">예상 콘텐츠가 검색 결과에 표시 되지 않을 경우 다음 문제 해결 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="f1e33-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="f1e33-104">필요한 콘텐츠가 포함 된 **사이트가** 검색 결과에 콘텐츠를 표시할 수 있도록 설정 되어 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="f1e33-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="f1e33-105">[검색 결과에서 사이트에 콘텐츠 표시](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)의 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="f1e33-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="f1e33-106">필요한 콘텐츠가 포함 된 **목록** 또는 **라이브러리가** 검색 결과에 콘텐츠를 표시할 수 있도록 설정 되어 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="f1e33-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="f1e33-107">[검색 결과에서 목록 또는 라이브러리의 콘텐츠 표시](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)에 있는 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="f1e33-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="f1e33-108">페이지, 문서 또는 사용자 지정 페이지 레이아웃이 **주 버전** 으로 게시 되었는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="f1e33-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="f1e33-109">검색에서 3 단계를 수행 하면 [SharePoint Online의 모든 결과가 반환 되지 않습니다](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="f1e33-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="f1e33-110">사용자에 게 콘텐츠를 볼 수 있는 **권한이** 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="f1e33-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="f1e33-111">[SharePoint에서 사용 권한 수준 이해](https://docs.microsoft.com/sharepoint/understanding-permission-levels)의 단계를 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="f1e33-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="f1e33-112">새 관리 속성을 추가 하 여 검색 스키마를 변경한 경우, 관리 속성을 편집 하거나, 관리 속성을 제거한 다음 크롤링을 요청 하 고 다시 인덱스를 변경 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f1e33-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="f1e33-113">[크롤링 수동 요청 및 사이트, 라이브러리 또는 목록에 대 한 다시 인덱싱](https://docs.microsoft.com/sharepoint/crawl-site-content)의 단계를 수행 하 여 콘텐츠를 **다시 색인화** 합니다.</span><span class="sxs-lookup"><span data-stu-id="f1e33-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="f1e33-114">이 작업은 시간이 다소 걸릴 수 있으며, 24 시간 정도 기다린 후에 결과를 다시 확인 하세요.</span><span class="sxs-lookup"><span data-stu-id="f1e33-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="f1e33-115">자세한 내용은 [사이트에서 콘텐츠를 검색할 수 있도록 설정을](https://docs.microsoft.com/sharepoint/make-site-content-searchable)참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="f1e33-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
