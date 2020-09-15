---
title: 콘텐츠 검색 결과 없음
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680653"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="74e5a-102">콘텐츠 검색/내보내기에서 결과 없음</span><span class="sxs-lookup"><span data-stu-id="74e5a-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="74e5a-103">콘텐츠 검색/내보내기 관련 문제는 특정 관리자가 설치 하 고 모든 관리자에 게 통신 하지는 않는 특정 준수 보안 필터로 인해 데이터를 반환 하지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="74e5a-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="74e5a-104">이 문제를 해결 하려면 다음과 같은 규정 준수 보안 필터가 있는지 확인 하십시오.</span><span class="sxs-lookup"><span data-stu-id="74e5a-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="74e5a-105">보안 및 준수 센터 Powershell에 연결</span><span class="sxs-lookup"><span data-stu-id="74e5a-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="74e5a-106">다음을 실행 합니다.</span><span class="sxs-lookup"><span data-stu-id="74e5a-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="74e5a-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="74e5a-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="74e5a-108">New-compliancesecurityfilter-조직 $org</span><span class="sxs-lookup"><span data-stu-id="74e5a-108">Get-ComplianceSecurityFilter -Organization $org</span></span>