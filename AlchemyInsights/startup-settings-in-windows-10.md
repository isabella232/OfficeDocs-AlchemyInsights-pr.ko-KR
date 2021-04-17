---
title: Windows 10의 시작 설정
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
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828158"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="ef03d-102">Windows 10의 시작 설정</span><span class="sxs-lookup"><span data-stu-id="ef03d-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="ef03d-103">**시작할 때 자동으로 실행되는 앱 변경**</span><span class="sxs-lookup"><span data-stu-id="ef03d-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="ef03d-104">시작 [> 앱 > 로 이동합니다.](ms-settings:startupapps?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="ef03d-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="ef03d-105">시작 시 실행할 앱이 켜져 있는지 **확인**</span><span class="sxs-lookup"><span data-stu-id="ef03d-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="ef03d-106">**시작할 때 자동으로 실행될 앱 추가**</span><span class="sxs-lookup"><span data-stu-id="ef03d-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="ef03d-107">시작을 **클릭하거나 탭하고** 시작할 때 실행할 앱을 찾아 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="ef03d-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="ef03d-108">앱을 마우스 오른쪽 단추로 클릭하고 추가 를 **클릭한** 다음 파일 위치 **열기 를 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="ef03d-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="ef03d-109">그러면 앱 바로 가기가 저장되는 위치가 열립니다.</span><span class="sxs-lookup"><span data-stu-id="ef03d-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="ef03d-110">파일 위치 열기 옵션이 없는 경우 시작 시 앱을 실행할 수 없음을 의미합니다.</span><span class="sxs-lookup"><span data-stu-id="ef03d-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="ef03d-111">파일 위치가 열리면 Windows 로고 키 **+ R을** 누르고 **shell:startup을** 입력한 다음 확인을 **클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="ef03d-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="ef03d-112">그러면 시작 폴더가 열립니다.</span><span class="sxs-lookup"><span data-stu-id="ef03d-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="ef03d-113">파일 위치에서 시작 폴더로 바로 가기를 복사하여 앱에 붙여넣습니다.</span><span class="sxs-lookup"><span data-stu-id="ef03d-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="ef03d-114">**고급 시작 옵션(안전 모드, UEFI 설정 및 다른 장치에서 부팅 포함)**</span><span class="sxs-lookup"><span data-stu-id="ef03d-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="ef03d-115">이러한 단계는 PC를 다시 시작하기 때문에 작업을 저장하고 열려 있는 문서를 닫습니다.</span><span class="sxs-lookup"><span data-stu-id="ef03d-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="ef03d-116">설정 > [업데이트 & 복구로 > 이동합니다.](ms-settings:recovery?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="ef03d-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="ef03d-117">고급 **시작에서** 지금 **다시 시작을 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="ef03d-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="ef03d-118">PC가 다시 시작된 후 옵션 선택 화면으로 다음을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="ef03d-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="ef03d-119">USB 드라이브와 같은 장치에서 부팅하려면 장치 **사용을 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="ef03d-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="ef03d-120">UEFI 설정(BIOS 설정이라고도 하는)을 입력하려면 **UEFI** 펌웨어 > 고급 옵션 > 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="ef03d-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="ef03d-121">안전 모드를 입력하거나 고급 시작 설정을 변경하려면 시작 > 고급 옵션 > 문제 해결을 클릭한 다음 다시 **시작을** **클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="ef03d-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="ef03d-122">[BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)복구 키를 입력해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ef03d-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="ef03d-123">PC를 다시 시작한 후 사용할 시작 설정을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="ef03d-123">After your PC restarts again, click the startup setting you want to use.</span></span>