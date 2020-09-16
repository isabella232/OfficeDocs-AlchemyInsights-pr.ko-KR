---
title: Windows 10의 시작 설정
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
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751141"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="05253-102">Windows 10의 시작 설정</span><span class="sxs-lookup"><span data-stu-id="05253-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="05253-103">**시작할 때 자동으로 실행 되는 앱 변경**</span><span class="sxs-lookup"><span data-stu-id="05253-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="05253-104">[시작 > 설정 > 앱](ms-settings:startupapps?activationSource=GetHelp)으로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="05253-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="05253-105">시작할 때 실행 하려는 앱 **이 켜져 있는지 확인 합니다.**</span><span class="sxs-lookup"><span data-stu-id="05253-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="05253-106">**시작할 때 자동으로 실행할 앱 추가**</span><span class="sxs-lookup"><span data-stu-id="05253-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="05253-107">**시작** 을 클릭 하거나 탭 하 여 시작할 때 실행 하려는 앱을 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="05253-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="05253-108">앱을 마우스 오른쪽 단추로 클릭 하 고 **자세히**를 클릭 한 다음 **파일 위치 열기**를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="05253-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="05253-109">이렇게 하면 앱 바로 가기가 저장 되는 위치가 열립니다.</span><span class="sxs-lookup"><span data-stu-id="05253-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="05253-110">열린 파일 위치에 대 한 옵션이 없는 경우에는 시작할 때 앱이 실행 될 수 없음을 의미 합니다.</span><span class="sxs-lookup"><span data-stu-id="05253-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="05253-111">파일 위치를 열고 **Windows 로고 키 + R**을 누르고 **shell: startup**을 입력 한 다음 **확인**을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="05253-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="05253-112">시작 폴더를 엽니다.</span><span class="sxs-lookup"><span data-stu-id="05253-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="05253-113">파일 위치에서 시작 폴더에 앱의 바로 가기를 복사 하 여 붙여 넣습니다.</span><span class="sxs-lookup"><span data-stu-id="05253-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="05253-114">**고급 시작 옵션 (안전 모드, UEFI 설정 및 다른 장치에서 부팅 포함)**</span><span class="sxs-lookup"><span data-stu-id="05253-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="05253-115">이 단계는 PC를 다시 시작 하므로 작업을 저장 하 고 열려 있는 문서를 모두 닫습니다.</span><span class="sxs-lookup"><span data-stu-id="05253-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="05253-116">[& 보안 > 복구를 업데이트 > 설정](ms-settings:recovery?activationSource=GetHelp)으로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="05253-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="05253-117">**고급 시작**에서 **지금 다시 시작**을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="05253-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="05253-118">PC를 다시 시작한 후 옵션 선택 화면에서 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="05253-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="05253-119">USB 드라이브와 같은 장치에서 부팅 하려면 **장치 사용**을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="05253-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="05253-120">UEFI 설정 (BIOS 설정)을 입력 하려면 **Uefi 펌웨어 설정 > > 고급 옵션 문제 해결**을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="05253-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="05253-121">안전 모드를 시작 하거나 고급 시작 설정을 변경 하려면 **문제 해결 > 고급 옵션 > 시작**을 클릭 한 다음 **다시 시작**을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="05253-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="05253-122">[BitLocker 복구 키](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)를 입력 하 라는 메시지가 표시 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="05253-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="05253-123">PC가 다시 시작 되 면 사용 하려는 시작 설정을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="05253-123">After your PC restarts again, click the startup setting you want to use.</span></span>