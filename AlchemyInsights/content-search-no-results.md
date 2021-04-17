---
title: 콘텐츠 검색 결과 없음
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816854"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="0670b-102">콘텐츠 검색/내보내기 결과 없음</span><span class="sxs-lookup"><span data-stu-id="0670b-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="0670b-103">콘텐츠 검색/내보내기에서 데이터가 반환되지 않는 문제는 특정 관리자가 설정한 특정 준수 보안 필터로 인해 일부 관리자에게 이를 전달하지 못하기 때문일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0670b-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="0670b-104">이 문제를 해결하기 위해 이 문제를 유발할 수 있는 준수 보안 필터가 없는지 확인하십시오.</span><span class="sxs-lookup"><span data-stu-id="0670b-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="0670b-105">보안 및 준수 센터 Powershell에 연결</span><span class="sxs-lookup"><span data-stu-id="0670b-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="0670b-106">다음 명령줄을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="0670b-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="0670b-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="0670b-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="0670b-108">Get-ComplianceSecurityFilter -Organization $org</span><span class="sxs-lookup"><span data-stu-id="0670b-108">Get-ComplianceSecurityFilter -Organization $org</span></span>