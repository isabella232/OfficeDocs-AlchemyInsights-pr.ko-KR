---
title: Windows 10에서 전원 또는 배터리 아이콘이 사라짐
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
- "9002953"
- "5655"
ms.openlocfilehash: 10213843f8ec5ceeaa191d3373406d767f2bea3c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771547"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a><span data-ttu-id="adb4b-102">Windows 10에서 전원 또는 배터리 아이콘이 사라짐</span><span class="sxs-lookup"><span data-stu-id="adb4b-102">Power or battery icon missing in Windows 10</span></span>

<span data-ttu-id="adb4b-103">Windows 10 디바이스에 배터리(예: 노트북 또는 태블릿 또는 USB를 통해 UPS에 연결된 PC)가 있는 경우 일반적으로 전원/배터리 아이콘이 시계 근처의 작업 표시줄에 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="adb4b-103">If your Windows 10 device has a battery (e.g., laptop or tablet, or a PC connected via USB to a UPS), normally a power/battery icon is shown in the taskbar near the clock, for example:</span></span>

![배터리 아이콘](media/battery-icon.png)

<span data-ttu-id="adb4b-105">이 아이콘이 표시되지 않으면 숨겨져 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="adb4b-105">If you don't see this icon, it may be hidden:</span></span>

1. <span data-ttu-id="adb4b-106">**[설정 > 개인 설정 > 작업 표시줄](ms-settings:taskbar?activationSource=GetHelp)** 로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="adb4b-106">Go to **[Settings > Personalization > Taskbar](ms-settings:taskbar?activationSource=GetHelp)**.</span></span>

2. <span data-ttu-id="adb4b-107">알림 영역에서 **작업 표시줄에 표시되는 아이콘 선택**을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="adb4b-107">In the Notification area, click **Select which icons appear on the taskbar**.</span></span>

3. <span data-ttu-id="adb4b-108">그런 다음 목록에서 **전원** 항목을 찾아 설정을 **켬**으로 전환합니다.</span><span class="sxs-lookup"><span data-stu-id="adb4b-108">Then find the **Power** item in the list and toggle its setting to **On**.</span></span>

    ![작업 표시줄에 전원 아이콘 표시](media/power-icon-on.png)

<span data-ttu-id="adb4b-110">**문제 해결**</span><span class="sxs-lookup"><span data-stu-id="adb4b-110">**Troubleshooting**</span></span>

<span data-ttu-id="adb4b-111">위의 지침을 따르고 **전원** 토글이 회색으로 표시되거나 표시되지 않는 경우, 작업 표시줄의 검색 상자에서 **디바이스 관리자**를 입력하고 결과 목록에서 **디바이스 관리자**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="adb4b-111">If you followed the above instructions and the **Power** toggle is greyed out or not visible, in the search box on the taskbar, type **device manager**, and then select **Device Manager** in the list of results.</span></span> <span data-ttu-id="adb4b-112">**배터리**에서 디바이스의 배터리를 마우스 오른쪽 단추로 클릭하고 **비활성화**를 클릭한 다음 **예**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="adb4b-112">Under **Batteries**, right-click the battery for your device, click **Disable**, and click **Yes**.</span></span> <span data-ttu-id="adb4b-113">몇 초 정도 기다린 다음, 배터리를 마우스 오른쪽 단추로 클릭하고 **활성화**를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="adb4b-113">Wait a few seconds, and then right-click the battery and click **Enable**.</span></span> <span data-ttu-id="adb4b-114">그러면 디바이스가 다시 시작됩니다.</span><span class="sxs-lookup"><span data-stu-id="adb4b-114">Then restart your device.</span></span>

<span data-ttu-id="adb4b-115">위의 지침을 수행했는데 여전히 배터리 아이콘이 작업 표시줄의 검색 상자에 표시되지 않는 경우, **작업 관리자**를 입력하고 결과 목록에서 **작업 관리자**를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="adb4b-115">If you followed the above instructions, but the battery icon does not appear on the taskbar, in the search box on the taskbar, type **task manager**, and then click **Task Manager** in the list of results.</span></span> <span data-ttu-id="adb4b-116">**이름**의 **프로세스** 탭에서 **Explorer**를 마우스 오른쪽 단추로 클릭하고 **다시 시작**을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="adb4b-116">On the **Processes** tab, under **Name**, right-click **Explorer**, and then click **Restart**.</span></span>
