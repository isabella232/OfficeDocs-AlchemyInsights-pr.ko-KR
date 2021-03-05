---
title: 보안 Exchange Server 정보
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005482"
- "9005483"
- "9413"
- "9412"
ms.openlocfilehash: 87a5cf1ac4dfb96a5406f6b1431adb6ead074fd6
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50449097"
---
# <a name="about-exchange-server-security-updates"></a><span data-ttu-id="7767c-102">보안 Exchange Server 정보</span><span class="sxs-lookup"><span data-stu-id="7767c-102">About Exchange Server Security updates</span></span>

<span data-ttu-id="7767c-103">Microsoft는 Exchange Server 중요한 보안 업데이트를 출시했습니다.</span><span class="sxs-lookup"><span data-stu-id="7767c-103">Microsoft has released a series of critical security updates for Exchange Server on-premises.</span></span> <span data-ttu-id="7767c-104">영향을 받는 서버 버전은 2010, Exchange Server, 2016 및 2019의 모든 업데이트 수준입니다.</span><span class="sxs-lookup"><span data-stu-id="7767c-104">The affected server versions are any update levels of Exchange Server 2010, 2013, 2016 and 2019.</span></span> <span data-ttu-id="7767c-105">Exchange Online은 영향을당하지 않지만 하이브리드 구성으로 인해 일부 사내 Exchange 서버가 있는 경우 잠재적으로 취약할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7767c-105">Exchange Online is NOT impacted, but if you have some on-premises Exchange servers due to Hybrid configuration, they are potentially vulnerable.</span></span>

<span data-ttu-id="7767c-106">프레미스 서버를 업데이트하기 위해 다음 버전의 Exchange 이상을 실행해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="7767c-106">To update your on-premises servers will have to be running at least the following versions of Exchange:</span></span>

- <span data-ttu-id="7767c-107">Exchange 2010 서비스 팩 3</span><span class="sxs-lookup"><span data-stu-id="7767c-107">Exchange 2010 Service Pack 3</span></span>
- <span data-ttu-id="7767c-108">Exchange Server 2013 CU 23</span><span class="sxs-lookup"><span data-stu-id="7767c-108">Exchange Server 2013 CU 23</span></span>
- <span data-ttu-id="7767c-109">Exchange Server 2016 CU 19 또는 CU 18</span><span class="sxs-lookup"><span data-stu-id="7767c-109">Exchange Server 2016 CU 19 or CU 18</span></span>
- <span data-ttu-id="7767c-110">Exchange Server 2019 CU 8 또는 CU 7</span><span class="sxs-lookup"><span data-stu-id="7767c-110">Exchange Server 2019 CU 8 or CU 7</span></span>

<span data-ttu-id="7767c-111">수정 위치는 다음 공지 사항을 [참조하세요. 릴리스: 2021년 3월](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901) Exchange Server 보안 업데이트</span><span class="sxs-lookup"><span data-stu-id="7767c-111">Please see the following announcement for location of fixes: [Released: March 2021 Exchange Server Security Updates](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)</span></span>

<span data-ttu-id="7767c-112">**중요 참고 사항:**</span><span class="sxs-lookup"><span data-stu-id="7767c-112">**Important notes:**</span></span>

<span data-ttu-id="7767c-113">위의 목록에 따라, 업데이트 설치가 작동하지 않는 경우, On-premises Servers are not running required Exchange versions.</span><span class="sxs-lookup"><span data-stu-id="7767c-113">Installation of updates will not work if your on-premises servers are not running required Exchange versions, as per the above list.</span></span>

<span data-ttu-id="7767c-114">수동으로 업데이트를 설치하는 경우 업데이트 KB 문서의 "알려진 문제" 섹션에서 중요한 정보를 확인하십시오.</span><span class="sxs-lookup"><span data-stu-id="7767c-114">If installing updates manually, please read the "Known issues" section of update KB articles for important information.</span></span> <span data-ttu-id="7767c-115">보안 업데이트는 상승된 CMD/PowerShell 프롬프트에서 실행해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="7767c-115">Security updates MUST be run from elevated CMD/PowerShell prompt!</span></span>
