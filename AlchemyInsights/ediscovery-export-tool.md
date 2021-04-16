---
title: eDiscovery 내보내기
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814594"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="6a1a6-102">eDiscovery 내보내기 도구를 설치하거나 실행할 수 없는 경우</span><span class="sxs-lookup"><span data-stu-id="6a1a6-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="6a1a6-103">eDiscovery 내보내기 도구를 설치하거나 실행하여 검색 결과를 다운로드할 수 없는 경우 다음을 검사합니다.</span><span class="sxs-lookup"><span data-stu-id="6a1a6-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="6a1a6-104">사용하는 컴퓨터가 다음의 선행 요구 사항을 충족합니다.</span><span class="sxs-lookup"><span data-stu-id="6a1a6-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="6a1a6-105">32비트 및 64비트 버전의 Windows 7 이상 버전</span><span class="sxs-lookup"><span data-stu-id="6a1a6-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="6a1a6-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="6a1a6-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="6a1a6-107">지원되는 브라우저:</span><span class="sxs-lookup"><span data-stu-id="6a1a6-107">A supported browser:</span></span>

  - <span data-ttu-id="6a1a6-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="6a1a6-108">Microsoft Edge</span></span>

    <span data-ttu-id="6a1a6-109">또는</span><span class="sxs-lookup"><span data-stu-id="6a1a6-109">Or</span></span>

  - <span data-ttu-id="6a1a6-110">Internet Explorer 10 이상 버전</span><span class="sxs-lookup"><span data-stu-id="6a1a6-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="6a1a6-111">Google Chrome 및 Mozilla Firefox와 같은 기타 브라우저는 지원되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="6a1a6-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="6a1a6-112">조직은 .blob.core.windows.net Azure의 끝점에 연결할 수 있습니다(와일드카드는 내보내기 작업의 고유 **\* 식별자를** 나타임).</span><span class="sxs-lookup"><span data-stu-id="6a1a6-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="6a1a6-113">Microsoft 365 보안 및 준수 센터에서 내보내기 역할이 &amp; 할당됩니다.</span><span class="sxs-lookup"><span data-stu-id="6a1a6-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="6a1a6-114">기본적으로 이 역할은 eDiscovery 관리자 역할 그룹에만 할당됩니다.</span><span class="sxs-lookup"><span data-stu-id="6a1a6-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="6a1a6-115">[eDiscovery 사용 권한 할당을 참조합니다.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)</span><span class="sxs-lookup"><span data-stu-id="6a1a6-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="6a1a6-116">자세한 내용은 콘텐츠 검색 결과 [내보내기 를 참조하세요.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)</span><span class="sxs-lookup"><span data-stu-id="6a1a6-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="6a1a6-117">100K 사서함을 내보낼 경우 내보내기 결과를 다운로드하려면 다음 Powershell을 사용하여  [100K](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)사서함에서 결과 내보내기 를 다운로드해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="6a1a6-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>