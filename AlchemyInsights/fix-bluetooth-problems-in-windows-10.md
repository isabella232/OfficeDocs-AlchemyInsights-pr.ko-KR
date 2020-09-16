---
title: Windows 10에서 Bluetooth 문제 해결
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
- "9001475"
- "3506"
ms.openlocfilehash: 7e7a397a1f6777972a81bcbb6bffa1c98d8370a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730165"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="eb102-102">Windows 10에서 Bluetooth 문제 해결</span><span class="sxs-lookup"><span data-stu-id="eb102-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="eb102-103">Bluetooth 아이콘이 없거나 Bluetooth를 켜거나 끌 수 없는 경우 Bluetooth 문제 해결사를 실행 하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="eb102-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="eb102-104">[문제 해결 설정을 열고](ms-settings:troubleshoot) **찾기 및 기타 문제 해결**에서 **Bluetooth** 를 클릭 한 다음 **문제 해결사 실행**을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="eb102-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="eb102-105">Bluetooth 아이콘이 표시 되지 않으면 bluetooth가 장치 관리자에 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="eb102-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="eb102-106">장치 관리자에서 **Bluetooth**를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="eb102-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="eb102-107">Bluetooth 어댑터 이름을 길게 누르거나 마우스 오른쪽 단추로 클릭 하 고 **장치 제거**를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="eb102-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="eb102-108">Windows 장치를 종료 하 고 몇 초간 기다린 후 다시 켭니다.</span><span class="sxs-lookup"><span data-stu-id="eb102-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="eb102-109">Windows에서 드라이버 다시 설치를 시도 합니다.</span><span class="sxs-lookup"><span data-stu-id="eb102-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="eb102-110">최근에 Windows 10 업데이트를 설치 했거나 Windows 10으로 업그레이드 한 경우 드라이버 업데이트를 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="eb102-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="eb102-111">장치 관리자에서 **bluetooth**를 클릭 하 고 bluetooth 어댑터 이름 ("라디오" 라는 단어를 포함할 수 있음)을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="eb102-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="eb102-112">Bluetooth 어댑터를 길게 누르거나 마우스 오른쪽 단추로 클릭 한 다음 **업데이트**드라이버  >  **소프트웨어를 자동으로 검색**을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="eb102-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="eb102-113">단계를 수행 하 고 **닫기를**클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="eb102-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="eb102-114">Windows에서 새 Bluetooth 드라이버를 찾을 수 없는 경우 PC 제조업체의 웹 사이트를 방문 하 여 최신 블루투스 드라이버를 다운로드 합니다.</span><span class="sxs-lookup"><span data-stu-id="eb102-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="eb102-115">다운로드 한 후에 **는 드라이버**  >  **소프트웨어에서 내 컴퓨터**에서 드라이버 파일을 검색 > 확인을 클릭 하  >  **Browse** **OK**  >  고**다음**단계를 수행 하 여 설치 합니다.</span><span class="sxs-lookup"><span data-stu-id="eb102-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="eb102-116">업데이트 된 드라이버를 설치한 후 컴퓨터를 다시 시작 하 고 연결 문제가 해결 되었는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="eb102-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="eb102-117">Bluetooth 문제를 해결 하는 방법에 대 한 자세한 내용은 [Windows 10에서의 Bluetooth 문제를 해결](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems)하는 전체 문서를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="eb102-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
