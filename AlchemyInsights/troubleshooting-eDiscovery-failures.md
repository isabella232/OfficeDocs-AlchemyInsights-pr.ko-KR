---
title: 1490-문제 해결-eDiscovery-실패
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
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277821"
---
# <a name="troubleshoot-content-search-errors"></a><span data-ttu-id="c0e3c-102">콘텐츠 검색 오류 문제 해결</span><span class="sxs-lookup"><span data-stu-id="c0e3c-102">Troubleshoot Content Search errors</span></span>

<span data-ttu-id="c0e3c-103">검색 결과를 내보낼 때 콘텐츠 검색에 문제가 발생 하거나 오류를 가져올 수 있습니까?</span><span class="sxs-lookup"><span data-stu-id="c0e3c-103">Are you experiencing problems with Content Search or getting failures when you export search results?</span></span>

<span data-ttu-id="c0e3c-104">예를 들어 검색을 실행할 때 다음 메시지가 수신 됩니까?</span><span class="sxs-lookup"><span data-stu-id="c0e3c-104">For example, are you receiving the following when running searches?</span></span>

- <span data-ttu-id="c0e3c-105">CS008 또는 CS012 오류</span><span class="sxs-lookup"><span data-stu-id="c0e3c-105">CS008 or CS012 errors</span></span>

- <span data-ttu-id="c0e3c-106">서버 사용 중/시간 제한 오류</span><span class="sxs-lookup"><span data-stu-id="c0e3c-106">Server busy/timeout errors</span></span>

- <span data-ttu-id="c0e3c-107">응용 프로그램 오류가 발생 했습니다.</span><span class="sxs-lookup"><span data-stu-id="c0e3c-107">Application error occurred</span></span>

<span data-ttu-id="c0e3c-108">또는 10만 사서함을 초과 하는 많은 수의 사서함에서 결과를 검색 하거나 내보낼 때 내보내기 오류가 발생 합니까?</span><span class="sxs-lookup"><span data-stu-id="c0e3c-108">Or when searching or exporting results from a large number of mailboxes (over 100,000 mailboxes), are you getting export errors?</span></span>

<span data-ttu-id="c0e3c-109">이러한 유형의 오류가 발생 하는 경우 실패 한 콘텐츠 위치에 대 한 검색을 다시 시도 합니다.</span><span class="sxs-lookup"><span data-stu-id="c0e3c-109">For these types of errors, retry the search for the content locations that have failed.</span></span> <span data-ttu-id="c0e3c-110">자세한 내용은  [이 문서](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) 를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="c0e3c-110">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>

<span data-ttu-id="c0e3c-111">10만 개 이상의 사서함을 내보내는 경우에는 다음 Powershell을 사용 하 여 내보내기 결과를 다운로드 해야 합니다 (  [10만 개 이상의 사서함에서 결과 내보내기](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)).</span><span class="sxs-lookup"><span data-stu-id="c0e3c-111">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>
