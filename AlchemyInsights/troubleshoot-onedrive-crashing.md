---
title: OneDrive 충돌 문제 해결
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
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665004"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="3d4bd-102">OneDrive 충돌 문제 해결</span><span class="sxs-lookup"><span data-stu-id="3d4bd-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="3d4bd-103">OneDrive가 반복적으로 충돌하는 경우 다음 문제 해결 단계를 시도해 보세요.</span><span class="sxs-lookup"><span data-stu-id="3d4bd-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="3d4bd-104">**레지스트리 키가 설정되어 있지 않은지 확인합니다.**</span><span class="sxs-lookup"><span data-stu-id="3d4bd-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="3d4bd-105">레지스트리 편집기를 사용해 HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="3d4bd-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="3d4bd-106">DisableFileSyncNGSC가 있고 1로 설정된 경우 키를 열고 값을 0으로 변경합니다.</span><span class="sxs-lookup"><span data-stu-id="3d4bd-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="3d4bd-107">시작으로 이동하여 수동으로 OneDrive를 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="3d4bd-107">Manually launch OneDrive by going to Start</span></span> ![Windows 키 누르기](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="3d4bd-109">검색 상자에 OneDrive를 입력하십시오. 그 다음 OneDrive 데스크톱 앱을 클릭하십시오.</span><span class="sxs-lookup"><span data-stu-id="3d4bd-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="3d4bd-110">**OneDrive 초기화:**</span><span class="sxs-lookup"><span data-stu-id="3d4bd-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="3d4bd-111">참고:</span><span class="sxs-lookup"><span data-stu-id="3d4bd-111">Notes:</span></span>

- <span data-ttu-id="3d4bd-112">OneDrive를 다시 설정하면 모든 기존 동기화 연결이 끊어집니다(개인용 OneDrive가 설정된 경우 개인 OneDrive 포함).</span><span class="sxs-lookup"><span data-stu-id="3d4bd-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="3d4bd-113">컴퓨터에서 OneDrive를 다시 설정해도 파일이나 데이터가 손실되지는 않습니다.</span><span class="sxs-lookup"><span data-stu-id="3d4bd-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="3d4bd-114">**OneDrive를 초기화하려면:**</span><span class="sxs-lookup"><span data-stu-id="3d4bd-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="3d4bd-115">Windows 키 와 R을 눌러 실행 대화 상자를 여세요.</span><span class="sxs-lookup"><span data-stu-id="3d4bd-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="3d4bd-116">%localappdata%\Microsoft\OneDrive\onedrive.exe /reset을 입력하고 확인을 누릅니다.</span><span class="sxs-lookup"><span data-stu-id="3d4bd-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="3d4bd-117">명령 창이 잠깐 나타날 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3d4bd-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="3d4bd-118">시작으로 이동하여 수동으로 OneDrive를 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="3d4bd-118">Manually launch OneDrive by going to Start</span></span> ![Windows 키 누르기](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="3d4bd-120">검색 상자에 OneDrive를 입력하십시오. 그 다음 OneDrive 데스크톱 앱을 클릭하십시오.</span><span class="sxs-lookup"><span data-stu-id="3d4bd-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="3d4bd-121">참고:</span><span class="sxs-lookup"><span data-stu-id="3d4bd-121">Notes:</span></span>

- <span data-ttu-id="3d4bd-122">다시 설정 전에 일부 폴더만 동기화하도록 선택한 경우 동기화가 완료되면 이 작업을 다시 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="3d4bd-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="3d4bd-123">자세한 내용은  [컴퓨터에 동기화할 OneDrive 폴더 선택](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) 을 읽어보세요.</span><span class="sxs-lookup"><span data-stu-id="3d4bd-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="3d4bd-124">개인용 OneDrive와 비즈니스용 OneDrive에 이 작업을 수행해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="3d4bd-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>