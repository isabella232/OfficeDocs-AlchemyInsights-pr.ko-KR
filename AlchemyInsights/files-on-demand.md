---
title: 요청 기반 파일 관리
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6432"
- "9003530"
ms.openlocfilehash: 846cda97ccd52fcb43ae4a44f73deeaaa6dc093d
ms.sourcegitcommit: b7bbe4c5419668ce8e84196db382032ca09cd176
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/08/2020
ms.locfileid: "47406592"
---
# <a name="configure-files-on-demand"></a><span data-ttu-id="18ffb-102">요청 기반 파일 관리 구성하기</span><span class="sxs-lookup"><span data-stu-id="18ffb-102">Configure Files On-Demand</span></span>

<span data-ttu-id="18ffb-103">OneDrive 요청 기반 파일 관리를 이용하면 파일을 다운로드하고 장치의 저장 공간을 사용하지 않아도 OneDrive의 모든 파일에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="18ffb-103">OneDrive Files On-Demand helps you access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

<span data-ttu-id="18ffb-104">PC에서 요청 기반 파일 관리를 구성하려면:</span><span class="sxs-lookup"><span data-stu-id="18ffb-104">To configure Files On-Demand on your PC:</span></span>

1. <span data-ttu-id="18ffb-105">Windows 작업 표시줄 알림 영역에서 흰색 또는 파란색 **OneDrive** 구름 아이콘을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="18ffb-105">Select the white or blue **OneDrive** cloud icon in the Windows taskbar notification area.</span></span> <span data-ttu-id="18ffb-106">**도움말 및 설정** 톱니바퀴 아이콘 > **설정**을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="18ffb-106">Select the **Help & Settings** gear icon > **Settings**.</span></span>
2. <span data-ttu-id="18ffb-107">**설정** 탭에서 **공간을 절약하고 사용할 때 파일 다운로드** 확인란을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="18ffb-107">On the **Settings** tab, select the **Save space and download files as you use them** box.</span></span>  

<span data-ttu-id="18ffb-108">레지스트리를 사용하여 요청 기반 파일 관리를 구성할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="18ffb-108">You can also configure Files On-Demand using the registry.</span></span>

<span data-ttu-id="18ffb-109">이 설정을 사용하지 않으면 Windows 10 사용자는 이전 버전의 Windows 사용자와 동일한 동기화 동작을 실행하며 요청 기반 파일 관리를 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="18ffb-109">If you disable this setting, Windows 10 users have the same sync behavior as users of previous versions of Windows, and aren't able to turn on Files On-Demand.</span></span> <span data-ttu-id="18ffb-110">이 설정을 구성하지 않으면 사용자는 요청 기반 파일 관리를 켜거나 끌 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="18ffb-110">If you do not configure this setting, users can turn Files On-Demand on or off.</span></span>

<span data-ttu-id="18ffb-111">이 정책을 사용하면 다음 레지스트리 키 값을 1로 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="18ffb-111">Enabling this policy sets the following registry key value to 1.</span></span> <span data-ttu-id="18ffb-112">이 정책을 사용하지 않으면 다음 레지스트리 키 값을 0으로 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="18ffb-112">Disabling this policy sets the following registry key value to 0.</span></span>

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

<span data-ttu-id="18ffb-113">“설정”에서 요청 기반 파일 관리 옵션을 볼 수 없는 경우 서비스 "Windows 클라우드 파일 필터 드라이버" 시작 유형이 2 (AUTO_START)로 설정되어 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="18ffb-113">If you can't see the Files On-Demand option in "Settings," make sure the service "Windows Cloud Files Filter Driver" start type is set to 2 (AUTO_START).</span></span> <span data-ttu-id="18ffb-114">이 기능을 사용하면 다음 레지스트리 키 값을 2로 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="18ffb-114">Enabling this feature sets the following registry key value to 2.</span></span>

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`