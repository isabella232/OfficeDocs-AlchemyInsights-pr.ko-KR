---
title: SharePoint Online의 검색
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f790efbe6ed445786933efa3fc980f974693d1d9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770773"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="06aa9-102">SharePoint Online의 콘텐츠 크롤링 및 인덱싱</span><span class="sxs-lookup"><span data-stu-id="06aa9-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="06aa9-103">사용자가 SharePoint Online에서 검색 내용을 찾을 수 있도록 콘텐츠를 크롤링한 후 검색 인덱스에 추가 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="06aa9-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span>

- <span data-ttu-id="06aa9-104">[사이트 콘텐츠를 검색 가능 하도록 설정](https://docs.microsoft.com/sharepoint/make-site-content-searchable)하 여 콘텐츠를 찾을 수 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="06aa9-104">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="06aa9-105">관리 속성을 변경 하거나 크롤링 속성과 관리 속성의 매핑을 변경한 후에는 변경 내용을 검색 인덱스에 반영 하기 전에 사이트를 다시 크롤링되 야 합니다.</span><span class="sxs-lookup"><span data-stu-id="06aa9-105">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span>

- <span data-ttu-id="06aa9-106">자세한 내용은 [사이트, 라이브러리 또는 목록에 대 한 크롤링 수동 요청과 다시 인덱싱](https://docs.microsoft.com/sharepoint/crawl-site-content)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="06aa9-106">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span>

- <span data-ttu-id="06aa9-107">크롤링을 수동으로 요청한 후 24 시간 이상 기다렸다가 전체 다시 인덱스를 만들어 문제가 발생 했는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="06aa9-107">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span>

- <span data-ttu-id="06aa9-108">크롤링을 시작한 후에 24 시간 이상이 통과 한 경우에는 지원 사례를 기록 하세요.</span><span class="sxs-lookup"><span data-stu-id="06aa9-108">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="06aa9-109">대부분의 경우 당사는 이미 해결 방법에 대한 작업을 하고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="06aa9-109">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="06aa9-110">솔루션을 완료 하려면 최소한 24 시간 이상 기다려 주세요.</span><span class="sxs-lookup"><span data-stu-id="06aa9-110">Please give us at least 24 hours to complete a solution.</span></span>

<span data-ttu-id="06aa9-111">**중요**: 사이트, 문서 (라이브러리) 또는 목록이 삭제 되었지만 여전히 검색 결과에 표시 되는 경우 사용자에 게 액세스 하려고 할 때 **오류 404 파일을 찾을 수 없습니다** . 라는 오류가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="06aa9-111">**Important**: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="06aa9-112">이 문제는 추가 조사를 위한 지원 사례로 기록해 야 합니다.</span><span class="sxs-lookup"><span data-stu-id="06aa9-112">This issue should be logged as a support case for further investigation.</span></span>



