---
title: 고급 헌팅 쿼리에 대한 모범 사례 적용
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568620"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="84388-102">고급 헌팅 쿼리에 대한 모범 사례 적용</span><span class="sxs-lookup"><span data-stu-id="84388-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="84388-103">복잡한 쿼리를 실행하는 동안 결과를 빠르게 처리하고 시간 제한을 방지하기 위해 다음과 같은 모범 사례를 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="84388-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="84388-104">새 쿼리를 시도할 때 항상 제한을 사용하여 결과 집합이 너무 크지 않도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="84388-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="84388-105">또한 결과 집합의 크기를 초기에 `count` 평가하는 데도 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="84388-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="84388-106">먼저 시간 필터를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="84388-106">Use time filters first.</span></span> <span data-ttu-id="84388-107">이상적으로는 쿼리를 7일로 제한하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="84388-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="84388-108">쿼리의 시작에서 시간 필터 바로 다음에 대부분의 데이터를 제거할 것으로 예상되는 필터를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="84388-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="84388-109">전체 토큰을 찾는 경우 대신 `has` 연산자를 사용 `contains` 합니다.</span><span class="sxs-lookup"><span data-stu-id="84388-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="84388-110">모든 열이 아닌 특정 열에서 검색을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="84388-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="84388-111">테이블을 조인할 때 먼저 행 수가 적은 테이블을 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="84388-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="84388-112">`project` 조인한 테이블의 필수 열만</span><span class="sxs-lookup"><span data-stu-id="84388-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="84388-113">자세한 내용은 고급 헌팅 쿼리 [모범 사례를 참조합니다.](https://go.microsoft.com/fwlink/?linkid=2144812)</span><span class="sxs-lookup"><span data-stu-id="84388-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>
