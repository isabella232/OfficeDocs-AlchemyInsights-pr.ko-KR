---
title: Windows 10에서 드라이브 공간 절약
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505362"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="0f34d-102">Windows 10에서 드라이브 공간 절약</span><span class="sxs-lookup"><span data-stu-id="0f34d-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="0f34d-103">Windows의 드라이브 공간을 절약하는 두 가지 옵션은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="0f34d-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="0f34d-104">Windows 10에서 드라이브 공간을 절약합니다.</span><span class="sxs-lookup"><span data-stu-id="0f34d-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="0f34d-105">외부 저장소 장치로 Windows 10 업데이트의 공간을 확장합니다.</span><span class="sxs-lookup"><span data-stu-id="0f34d-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="0f34d-106">디스크 정리를 사용한 후에도 디스크 공간이 여전히 부족한 경우 Temp 폴더가 Microsoft 스토어에서 사용하는 응용 프로그램(.appx) 파일로 빠르게 채워질 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0f34d-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="0f34d-107">이 문제를 해결하려면 스토어를 다시 설정하고 스토어 캐시를 지운 다음 Windows 업데이트 문제 해결사 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="0f34d-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="0f34d-108">다음 단계를 진행하기 전에 Microsoft 스토어를 닫아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0f34d-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="0f34d-109">**1단계: Microsoft 스토어 다시 설정**</span><span class="sxs-lookup"><span data-stu-id="0f34d-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="0f34d-110">**참고** 기본 설정 및 로그인 세부 정보를 포함하여 장치에서 앱 데이터가 영구적으로 삭제됩니다.</span><span class="sxs-lookup"><span data-stu-id="0f34d-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="0f34d-111">**시작** > **설정** > **앱** > **앱 및 기능** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="0f34d-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="0f34d-112">앱 목록에서 Microsoft 스토어를 찾아 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="0f34d-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="0f34d-113">**고급 옵션을** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="0f34d-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="0f34d-114">아래로 스크롤하고 **다시 설정** 을 선택한 후 **다시 설정 확인을** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="0f34d-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="0f34d-115">**2단계: Microsoft 스토어 캐시 지우기**</span><span class="sxs-lookup"><span data-stu-id="0f34d-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="0f34d-116">Windows 로고 키 + R을 눌러 실행 대화 상자를 열 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0f34d-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="0f34d-117">wsreset.exe를 입력하고 **확인** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="0f34d-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="0f34d-118">빈 명령 프롬프트 창이 열립니다.</span><span class="sxs-lookup"><span data-stu-id="0f34d-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="0f34d-119">약 10초 후에 창이 닫히고 스토어가 자동으로 열립니다.</span><span class="sxs-lookup"><span data-stu-id="0f34d-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="0f34d-120">**3단계: Windows 업데이트 다시 설정**</span><span class="sxs-lookup"><span data-stu-id="0f34d-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="0f34d-121">**시작** > **설정** > **업데이트 및 보안** > **문제해결** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="0f34d-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="0f34d-122">아래로 스크롤하여 목록에서 **Windows 업데이트** 를 선택한 다음, **문제해결사 실행** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="0f34d-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="0f34d-123">컴퓨터를 다시부팅하고 여전히 문제가 발생하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="0f34d-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

