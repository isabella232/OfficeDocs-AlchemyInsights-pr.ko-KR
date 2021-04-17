---
title: 기존 모니터 문제 해결
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
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824585"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="7d06f-102">기존 모니터 문제 해결</span><span class="sxs-lookup"><span data-stu-id="7d06f-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="7d06f-103">이러한 해결 방법을 시도하여 모니터 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="7d06f-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="7d06f-104">**모니터 디스플레이를 새로 고치기:**</span><span class="sxs-lookup"><span data-stu-id="7d06f-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="7d06f-105">Windows 키 + Ctrl + Shift + B 키를 동시에 누르고 있습니다. 이렇게 하면 그래픽 드라이버와의 통신이 새로 고쳐지게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="7d06f-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="7d06f-106">모니터가 잠시 깜박이고 몇 초 후에 돌아올 것입니다.</span><span class="sxs-lookup"><span data-stu-id="7d06f-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="7d06f-107">**모니터 하드웨어 문제 해결:**</span><span class="sxs-lookup"><span data-stu-id="7d06f-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="7d06f-108">PC를 모니터에 연결하는 케이블의 플러그를 뽑았다가 다시 꽂습니다.</span><span class="sxs-lookup"><span data-stu-id="7d06f-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="7d06f-109">PC에서 필수적이지 않은 장치(예: 어댑터 또는 도크)의 연결을 끊습니다.</span><span class="sxs-lookup"><span data-stu-id="7d06f-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="7d06f-110">**최근에 PC에 업데이트를 설치한 경우 디스플레이 드라이버를 롤백할 수 있습니다.**</span><span class="sxs-lookup"><span data-stu-id="7d06f-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="7d06f-111">시작을 선택하고 **장치 관리자를** 입력하고 결과에서 **장치** 관리자를 선택합니다. </span><span class="sxs-lookup"><span data-stu-id="7d06f-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="7d06f-112">디스플레이 어댑터 **섹션을** 확장하고 디스플레이 어댑터를 마우스 오른쪽 단추로 클릭한 다음 속성을 **선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="7d06f-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="7d06f-113">드라이버 **탭으로 이동하여** 드라이버 **롤백을 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="7d06f-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="7d06f-114">참고: 사용할 수 없는 경우 또는 회색으로 표시될 경우 아래 옵션에서 **아니요를** 선택하여 다음 단계로 이동하세요.</span><span class="sxs-lookup"><span data-stu-id="7d06f-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="7d06f-115">이러한 변경 내용이 적용되기 전에 PC를 다시 시작해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7d06f-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="7d06f-116">**디스플레이 드라이버를 제거하고 다시 설치합니다.**</span><span class="sxs-lookup"><span data-stu-id="7d06f-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="7d06f-117">시작을 선택하고 **장치 관리자를** 입력하고 결과에서 **장치** 관리자를 선택합니다. </span><span class="sxs-lookup"><span data-stu-id="7d06f-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="7d06f-118">디스플레이 어댑터 **섹션을** 확장하고 디스플레이 어댑터를 마우스 오른쪽 단추로 클릭한 다음 장치 **제거를 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="7d06f-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="7d06f-119">이 장치에 대한 드라이버 소프트웨어 삭제 옆의 **상자를 선택하고** 제거 **를 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="7d06f-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="7d06f-120">참고: 이 단계에서 컴퓨터를 다시 시작해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7d06f-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="7d06f-121">다시 시작하기 전에 나머지 지침을 적어 두십시오.</span><span class="sxs-lookup"><span data-stu-id="7d06f-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="7d06f-122">장치 관리자를 다시 니다.</span><span class="sxs-lookup"><span data-stu-id="7d06f-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="7d06f-123">디스플레이 어댑터 **섹션을** 확장하고 디스플레이 어댑터를 마우스 오른쪽 단추로 클릭한 다음 **드라이버 업데이트를 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="7d06f-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="7d06f-124">드라이버 **소프트웨어 업데이트 자동 검색을 선택하고** 설치 지침을 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="7d06f-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>