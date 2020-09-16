---
title: Windows 10에서 Windows 메모리 진단 실행
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: f2b8306d0cd604b144b82275243c5a84580bc609
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720796"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="8478c-102">Windows 10에서 Windows 메모리 진단 실행</span><span class="sxs-lookup"><span data-stu-id="8478c-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="8478c-103">PC에서 Windows 및 앱이 작동을 중지하거나 멈추거나 또는 불안정한 방식으로 작동하는 경우 PC의 메모리(RAM)에 문제가 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8478c-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="8478c-104">Windows 메모리 진단 도구를 실행하 여 PC의 RAM 문제를 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8478c-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="8478c-105">작업 표시줄의 검색 상자에 **메모리 진단**을 입력한 다음, **Windows 메모리 진단**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="8478c-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="8478c-106">진단 도구를 실행하려면 PC를 다시 시작해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="8478c-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="8478c-107">즉시 다시 시작하는 옵션(작업을 저장 하고 열린 문서와 전자 메일을 먼저 닫음)을 사용하거나 다음에 PC가 다시 시작될 때 진단이 자동으로 실행되도록 예약하는 옵션이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8478c-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Windows 메모리 진단](media/windows-memory-diagnostic.png)

<span data-ttu-id="8478c-109">PC가 다시 시작될 때, **Windows 메모리 진단 도구**가 자동으로 실행됩니다.</span><span class="sxs-lookup"><span data-stu-id="8478c-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="8478c-110">진단 도구가 실행되는 동안 상태와 진행률이 표시되고 키보드에서 **ESC** 키를 눌러 진단 도구를 취소할 수 있는 옵션이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8478c-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="8478c-111">진단이 완료되면 Windows가 정상적으로 시작됩니다.</span><span class="sxs-lookup"><span data-stu-id="8478c-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="8478c-112">다시 시작된 직후에 바탕 화면이 나타나면 작업 표시줄에서 **알림 센터** 아이콘 옆에 알림이 표시되어 메모리 오류를 찾았는지 여부를 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="8478c-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="8478c-113">예시:</span><span class="sxs-lookup"><span data-stu-id="8478c-113">For example:</span></span>

<span data-ttu-id="8478c-114">알림 센터 아이콘은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="8478c-114">Here's the Action Center icon:</span></span> ![알림 센터 아이콘](media/action-center-icon.png) 

<span data-ttu-id="8478c-116">샘플 알림:</span><span class="sxs-lookup"><span data-stu-id="8478c-116">And a sample notification:</span></span> ![메모리 오류 없음](media/no-memory-errors.png)

<span data-ttu-id="8478c-118">알림을 놓친 경우, 작업 표시줄에 있는 **알림 센터** 아이콘을 선택하여 **알림 센터**를 표시하고 스크롤할 수 있는 알림 목록을 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8478c-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="8478c-119">세부 정보를 검토하려면 작업 표시줄의 검색 상자에 **이벤트**를 입력한 다음, **이벤트 뷰어**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="8478c-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="8478c-120">**이벤트 뷰어의 왼쪽 창에서\*\*\*\*Windows 로그 > 시스템**으로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="8478c-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="8478c-121">오른쪽 창에서 원본값 **MemoryDiagnostics-Results**가 있는 이벤트를 볼 때까지 **원본** 열을 보며 목록 아래로 검색합니다.</span><span class="sxs-lookup"><span data-stu-id="8478c-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="8478c-122">해당되는 각 이벤트를 강조 표시하고 목록 아래의 **일반** 탭 아래에 있는 상자에서 결과 정보를 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="8478c-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
