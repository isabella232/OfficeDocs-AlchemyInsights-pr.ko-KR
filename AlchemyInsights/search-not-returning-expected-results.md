---
title: 1491-검색이 예상 대로 반환 되지 않음-결과
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740480"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="18c3b-102">콘텐츠 검색에서 필요한 결과를 반환 하지 않음</span><span class="sxs-lookup"><span data-stu-id="18c3b-102">Content Search not returning expected results</span></span>

<span data-ttu-id="18c3b-103">Microsoft 365 보안 & 준수 센터에서 콘텐츠 검색을 실행 하는 경우 예기치 않은 검색 결과가 나타날 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="18c3b-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="18c3b-104">검색 결과에 영향을 줄 수 있는 다음과 같은 사항을 고려 하십시오.</span><span class="sxs-lookup"><span data-stu-id="18c3b-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="18c3b-105">**콘텐츠 위치 및 검색 조건**: 적절 한 콘텐츠 위치 및 검색 조건을 선택 했는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="18c3b-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="18c3b-106">여러 위치에서 큰 검색을 실행 한 경우에는 여러 검색으로 분할 하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="18c3b-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="18c3b-107">**부분적으로 인덱싱된 항목**: 사서함에서  [부분적으로 인덱싱된 항목이](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) 예상 검색 결과에 포함 됩니다.</span><span class="sxs-lookup"><span data-stu-id="18c3b-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="18c3b-108">그러나 SharePoint 및 OneDrive의 사이트에서 부분적으로 인덱싱된 항목은 검색 예상에 포함 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="18c3b-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="18c3b-109">**검색 실패**: 10만 사서함을 초과 하 여 많은 수의 사서함을 검색 하는 경우 CS008-009 및 CS012-002와 같은 오류 코드를 사용 하 여 검색 오류를 가져올 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="18c3b-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="18c3b-110">이 경우 실패 한 콘텐츠 위치에 대해서만 검색을 다시 시도 합니다.</span><span class="sxs-lookup"><span data-stu-id="18c3b-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="18c3b-111">자세한 내용은  [이 문서](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) 를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="18c3b-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
