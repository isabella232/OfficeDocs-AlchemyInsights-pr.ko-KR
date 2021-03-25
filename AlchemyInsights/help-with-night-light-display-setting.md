---
title: 야간 표시 설정 도움말
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123142"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="029b1-102">야간 표시 설정 도움말</span><span class="sxs-lookup"><span data-stu-id="029b1-102">Help with the night light display setting</span></span>

<span data-ttu-id="029b1-103">야간 표시 설정에 대한 자세한 내용은 [Windows 10에서 야간 표시 설정](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="029b1-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="029b1-104">설정에서 야간 조명 옵션이 회색으로 표시된 경우 디스플레이 드라이버를 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="029b1-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="029b1-105">작업 표시줄의 검색 상자를 클릭하고 **장치 관리자** 를 입력한 다음 검색 결과에서 **장치 관리자** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="029b1-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="029b1-106">**어댑터 표시** 를 확장합니다.</span><span class="sxs-lookup"><span data-stu-id="029b1-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="029b1-107">장치가 DisplayLink 드라이버 또는 Basic Display 드라이버를 사용하는 경우에는 야간 조명 기능을 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="029b1-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="029b1-108">야간 조명 기능은 최신 그래픽 기술을 활용하므로 디스플레이 드라이버를 업데이트해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="029b1-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="029b1-109">**시작** > **설정** > **업데이트 및 보안** > **Windows 업데이트** > **업데이트 확인** 으로 이동하여 업데이트를 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="029b1-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="029b1-110">또는</span><span class="sxs-lookup"><span data-stu-id="029b1-110">OR</span></span>

- <span data-ttu-id="029b1-111">하드웨어 제조업체의 지원 웹 사이트를 방문하여 최신 디스플레이 드라이버를 수동으로 다운로드하고 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="029b1-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="029b1-112">레지스트리의 야간 표시등 다시 설정</span><span class="sxs-lookup"><span data-stu-id="029b1-112">Reset night light in the registry</span></span>

<span data-ttu-id="029b1-113">디스플레이 드라이버를 업데이트하지 못한 경우 레지스트리에서 야간 조명을 재설정해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="029b1-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="029b1-114">**주의:** 이 문제 해결 단계는 고급 사용자에게만 권장됩니다.</span><span class="sxs-lookup"><span data-stu-id="029b1-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="029b1-115">레지스트리를 잘못 수정하는 경우 심각한 문제가 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="029b1-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="029b1-116">추가 보호를 위해 문제가 발생한 경우 복원할 수 있도록 레지스트리를 수정하기 전에 백업하세요.</span><span class="sxs-lookup"><span data-stu-id="029b1-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="029b1-117">검색 상자에 **regedit** 을 입력하고 검색 결과에 **레지스트리 편집기** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="029b1-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="029b1-118">다음 레지스트리 키로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="029b1-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="029b1-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="029b1-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="029b1-120">내보내고 $$windows.data.bluelightreduction.bluelightreductionstate 하위 키를 삭제합니다.</span><span class="sxs-lookup"><span data-stu-id="029b1-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="029b1-121">내보내고 $$windows.data.bluelightreduction.settings 하위 키를 삭제합니다.</span><span class="sxs-lookup"><span data-stu-id="029b1-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="029b1-122">Windows를 다시 시작하고 야간 표시등 옵션을 사용할 수 있는지 여부를 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="029b1-122">Restart Windows and verify if the night light options are available.</span></span>


