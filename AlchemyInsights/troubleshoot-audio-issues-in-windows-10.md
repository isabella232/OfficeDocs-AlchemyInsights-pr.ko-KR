---
title: Windows 10의 오디오 문제 해결
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
- "3476"
- "9001463"
ms.openlocfilehash: 88157f9c82bc970e989d47f5cf376b7ce485cb2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750314"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="46bf4-102">Windows 10의 오디오 문제 해결</span><span class="sxs-lookup"><span data-stu-id="46bf4-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="46bf4-103">**오디오 문제 해결사 실행**</span><span class="sxs-lookup"><span data-stu-id="46bf4-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="46bf4-104">[문제 해결 설정을](ms-settings:troubleshoot)엽니다.</span><span class="sxs-lookup"><span data-stu-id="46bf4-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="46bf4-105">**오디오 재생**  >  **을 선택 하 여 문제 해결사를 실행**합니다.</span><span class="sxs-lookup"><span data-stu-id="46bf4-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="46bf4-106">**기본 장치 설정**</span><span class="sxs-lookup"><span data-stu-id="46bf4-106">**Set the default device**</span></span>

<span data-ttu-id="46bf4-107">USB 또는 HDMI를 사용 하 여 오디오 장치에 연결 하는 경우 해당 장치를 기본값으로 설정 해야 할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="46bf4-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="46bf4-108">소리 **시작**  >  **Sound**을 열고 **소리** 를 선택 하거나 결과 목록에서 **시스템 소리를 변경** 합니다.</span><span class="sxs-lookup"><span data-stu-id="46bf4-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="46bf4-109">**재생** 탭에서 장치를 선택 하 고 **기본값 설정을**선택한 다음 **확인**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="46bf4-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="46bf4-110">**케이블, 볼륨, 스피커 및 헤드폰 확인**</span><span class="sxs-lookup"><span data-stu-id="46bf4-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="46bf4-111">스피커 및 헤드폰 연결에서 케이블이 제대로 연결 되었는지 확인 하 고 케이블 연결이 올바른지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="46bf4-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="46bf4-112">전원 및 볼륨 수준을 확인 하 고 모든 볼륨 컨트롤을 켜십시오.</span><span class="sxs-lookup"><span data-stu-id="46bf4-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="46bf4-113">일부 스피커와 앱에는 자체 볼륨 컨트롤이 있습니다. 해당 사용자를 모두 확인 하 여 적절 한 수준으로 설정 해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="46bf4-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="46bf4-114">다른 USB 포트를 사용 하 여 연결 해 봅니다.</span><span class="sxs-lookup"><span data-stu-id="46bf4-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="46bf4-115">**참고**: 헤드폰이 연결 되어 있으면 스피커가 작동 하지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="46bf4-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="46bf4-116">**장치 관리자 확인**</span><span class="sxs-lookup"><span data-stu-id="46bf4-116">**Check Device Manager**</span></span>

<span data-ttu-id="46bf4-117">드라이버의 최신 상태를 확인 하려면 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="46bf4-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="46bf4-118">**시작**을 선택 하 고 **장치 관리자**를 입력 한 다음 결과 목록에서 **장치 관리자** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="46bf4-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="46bf4-119">**사운드, 비디오 및 게임 컨트롤러**에서 사운드 카드를 선택 하 고 열고 **드라이버** 탭을 선택한 다음 **드라이버 업데이트**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="46bf4-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="46bf4-120">**참고**: Windows에서 새 드라이버를 찾지 못하는 경우 장치 제조업체의 웹 사이트에서 검색 한 다음 해당 지침을 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="46bf4-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="46bf4-121">**드라이버 다시 설치**</span><span class="sxs-lookup"><span data-stu-id="46bf4-121">**Reinstall the driver**</span></span>

<span data-ttu-id="46bf4-122">장치 관리자를 통해 업데이트할 수 없거나 제조업체의 웹 사이트에서 새 드라이버를 찾지 못하는 경우 다음 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="46bf4-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="46bf4-123">장치 관리자에서 오디오 드라이버를 마우스 오른쪽 단추로 클릭 하거나 길게 누른 다음 **제거**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="46bf4-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="46bf4-124">장치를 다시 시작 하면 Windows에서 드라이버 다시 설치를 시도 합니다.</span><span class="sxs-lookup"><span data-stu-id="46bf4-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="46bf4-125">드라이버가 제대로 설치 되지 않은 경우 Windows와 함께 제공 되는 일반 오디오 드라이버를 사용해 보십시오.</span><span class="sxs-lookup"><span data-stu-id="46bf4-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="46bf4-126">장치 관리자에서 오디오 > 드라이버를 마우스 오른쪽 단추로 클릭 (또는 길게 누르기) 하 **고, 드라이버**소프트웨어  >  **를 검색**하 여 내 컴퓨터  >  **의 장치 드라이버 목록에서**선택한 **다음, 다음**을 선택 하 고 **High Definition Audio Device**지침에 따라 설치 합니다.</span><span class="sxs-lookup"><span data-stu-id="46bf4-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>
