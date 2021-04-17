---
title: 일정 이벤트가 누락되거나 업데이트되지 않는 경우
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10932"
- "9001435"
ms.openlocfilehash: b114411d6285a68a41bbcbf64151c212ee2cf661
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819982"
---
# <a name="calendar-events-missing-or-not-updating"></a><span data-ttu-id="c943c-102">일정 이벤트가 누락되거나 업데이트되지 않는 경우</span><span class="sxs-lookup"><span data-stu-id="c943c-102">Calendar Events missing or not updating</span></span>

<span data-ttu-id="c943c-103">일정 항목이 누락되거나 업데이트되지 않는 경우 먼저 Outlook의 일정 폴더 속성에서 항목 개수를 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="c943c-103">If calendar items are missing or not updating, start by looking at the item count in your Calendar folder properties in Outlook:</span></span> 

1. <span data-ttu-id="c943c-104">영향을 받는 사용자의 **일정** 폴더를 마우스 오른쪽 단추로 클릭한 다음 **속성을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="c943c-104">Right-click on the affected user **Calendar** folder, and then select **Properties**.</span></span>

1. <span data-ttu-id="c943c-105">**동기화** 탭을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="c943c-105">Select the **Synchronization** tab.</span></span>

<span data-ttu-id="c943c-106">서버 폴더와 오프라인 폴더 간에 항목 수가 같지 않은 경우:</span><span class="sxs-lookup"><span data-stu-id="c943c-106">If the item count is not the same between the Server folder and the Offline Folder:</span></span>

1.  <span data-ttu-id="c943c-107">**일정** 폴더를 강조 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="c943c-107">Highlight the **Calendar** folder.</span></span>

1.  <span data-ttu-id="c943c-108">**보내기**/**수신** 탭으로 이동한 다음 **폴더 업데이트** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="c943c-108">Go to the **Send**/**Receive** tab, and then select **Update Folder**.</span></span>

<span data-ttu-id="c943c-109">일정이 여전히 업데이트되지 않거나 이벤트가 누락되는 경우 [Microsoft 다운로드 센터](https://www.microsoft.com/download/details.aspx?id=28786)에서 Outlook용 일정 확인 도구를 다운로드합니다.</span><span class="sxs-lookup"><span data-stu-id="c943c-109">If your calendar is still not updating or events are missing, download the Calendar Checking Tool for Outlook from the [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=28786).</span></span> <span data-ttu-id="c943c-110">일정 폴더에 5,000개 이상의 항목이 있는지 확인합니다. 그러한 경우 일정 모임이 업데이트되지 않거나 모임 오류와 같은 증상을 일으킬 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c943c-110">Determine if there are more than 5000 items in the calendar folder as this can cause symptoms such as calendar meetings not updated or meeting errors.</span></span> 

<span data-ttu-id="c943c-111">자세한 내용은 [캐시된 모드 .ost 혹은 .pst 파일에 너무 많은 항목 또는 폴더가 있는 경우 Outlook 성능 문제](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c943c-111">For more information, see [Outlook performance issues when there are too many items or folders in a cached mode .ost or .pst file](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders).</span></span>