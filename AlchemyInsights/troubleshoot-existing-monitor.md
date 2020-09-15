---
title: 기존 모니터 문제 해결
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
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690717"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="6c169-102">기존 모니터 문제 해결</span><span class="sxs-lookup"><span data-stu-id="6c169-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="6c169-103">다음 솔루션을 사용해 서 모니터 문제를 해결 해 보세요.</span><span class="sxs-lookup"><span data-stu-id="6c169-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="6c169-104">**모니터 화면을 새로 고칩니다.**</span><span class="sxs-lookup"><span data-stu-id="6c169-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="6c169-105">Windows 키 + Ctrl + Shift + B와 같은 시간에 다음 키를 동시에 누릅니다. 이렇게 하면 그래픽 드라이버와의 통신이 새로 고쳐집니다.</span><span class="sxs-lookup"><span data-stu-id="6c169-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="6c169-106">모니터가 잠시 깜박이 며 몇 초 후에 다시 돌아올 것입니다.</span><span class="sxs-lookup"><span data-stu-id="6c169-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="6c169-107">**모니터 하드웨어 문제 해결:**</span><span class="sxs-lookup"><span data-stu-id="6c169-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="6c169-108">PC를 모니터에 연결 하는 케이블을 뽑은 다음 다시 연결 합니다.</span><span class="sxs-lookup"><span data-stu-id="6c169-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="6c169-109">PC에서 중요 하지 않은 모든 장치 (예: 어댑터나 도킹 회사)의 연결을 끊습니다.</span><span class="sxs-lookup"><span data-stu-id="6c169-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="6c169-110">**최근에 PC에 업데이트를 설치한 경우 디스플레이 드라이버를 롤백할 수 있습니다.**</span><span class="sxs-lookup"><span data-stu-id="6c169-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="6c169-111">**시작**을 선택 하 고 **장치 관리자**를 입력 한 다음 결과에서 **장치 관리자** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="6c169-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="6c169-112">**디스플레이 어댑터** 섹션을 확장 하 고, 디스플레이 어댑터를 마우스 오른쪽 단추로 클릭 한 다음 and 조합해 **속성**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="6c169-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="6c169-113">**드라이버** 탭으로 이동 하 여 **드라이버 롤백을**선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="6c169-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="6c169-114">참고:이 매개 변수를 사용할 수 없거나 회색으로 표시 된 경우 아래 옵션에서 **아니요** 를 선택 하 여 다음 단계로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="6c169-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="6c169-115">이 변경 내용을 적용 하려면 PC를 다시 시작 해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6c169-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="6c169-116">**디스플레이 드라이버를 제거 하 고 다시 설치 합니다.**</span><span class="sxs-lookup"><span data-stu-id="6c169-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="6c169-117">**시작**을 선택 하 고 **장치 관리자**를 입력 한 다음 결과에서 **장치 관리자** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="6c169-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="6c169-118">**디스플레이 어댑터** 섹션을 확장 하 고 and 조합해 디스플레이 어댑터를 마우스 오른쪽 단추로 클릭 한 다음 **장치 제거**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="6c169-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="6c169-119">**이 장치에 대 한 드라이버 소프트웨어 삭제** 옆의 확인란을 선택 하 고 **제거**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="6c169-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="6c169-120">참고:이 단계에서 컴퓨터를 다시 시작 하 라는 메시지가 표시 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6c169-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="6c169-121">다시 시작 하기 전에 나머지 지침을 적어 두어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="6c169-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="6c169-122">장치 관리자를 다시 엽니다.</span><span class="sxs-lookup"><span data-stu-id="6c169-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="6c169-123">**디스플레이 어댑터** 섹션을 확장 하 고 디스플레이 어댑터를 마우스 오른쪽 단추로 클릭 한 다음 **드라이버 업데이트**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="6c169-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="6c169-124">**업데이트 드라이버 소프트웨어 자동으로 검색** 을 선택 하 고 설치 지침을 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="6c169-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>