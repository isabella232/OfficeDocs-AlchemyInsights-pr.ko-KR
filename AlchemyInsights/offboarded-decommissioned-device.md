---
title: 장치 인벤토리에서 오프보딩되거나 해제된 장치를 제거하는 데 문제가 있습니다.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/11/2021
ms.locfileid: "52319176"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a><span data-ttu-id="aaa5d-102">장치 인벤토리에서 오프보딩되거나 해제된 장치를 제거하는 데 문제가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="aaa5d-102">Issues with removing an offboarded or decommissioned device from the Device Inventory</span></span>

<span data-ttu-id="aaa5d-103">끝점용 Microsoft Defender는 현재 장치 인벤토리에서 오프보딩 또는 해제된 장치의 장치 레코드를 수동으로 제거할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="aaa5d-103">Microsoft Defender for Endpoint does not currently allow manually removing the device record of an offboarded or decommissioned device from the Device Inventory.</span></span>

<span data-ttu-id="aaa5d-104">보안을 위해 장치는 포털에 최대 180일 동안 기록 레코드로 남아 있습니다.</span><span class="sxs-lookup"><span data-stu-id="aaa5d-104">For security purposes, the device remains in the portal as an historical record for up to 180 days.</span></span> <span data-ttu-id="aaa5d-105">그러나 구성된 보존 기간에 따라 장치 데이터가 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="aaa5d-105">However, the device data is purged according to your configured retention period.</span></span>

<span data-ttu-id="aaa5d-106">**참고:** 오프보딩되거나 해제된 장치는 7일  후에 자동으로 비활성 상태로 전환됩니다.</span><span class="sxs-lookup"><span data-stu-id="aaa5d-106">**Note:** An offboarded or decommissioned device switches automatically to **Inactive** state after seven days.</span></span> <span data-ttu-id="aaa5d-107">또한 지난 30일 동안 활성화되지 않은 장치는 조직 위협 및 취약성 관리 노출 점수 또는 장치용 Microsoft 보안 점수를 반영하는 데이터에 반영되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="aaa5d-107">In addition, devices not active in the last 30 days are not factored into the data that reflects your organization threat and vulnerability management exposure score or Microsoft Secure Score for Devices.</span></span>
 
<span data-ttu-id="aaa5d-108">여전히 장치 인벤토리 보기에서 특정 장치를 보고 싶지 않은 경우 장치 태그를 배치하여 장치 인벤토리 보기에서 해제된 장치를 필터링해 봐야 합니다.</span><span class="sxs-lookup"><span data-stu-id="aaa5d-108">If you still don't want to see certain devices in Device Inventory view, try placing a device tag to filter out the decommissioned device from the Device Inventory view.</span></span>

<span data-ttu-id="aaa5d-109">자세한 내용은 다음을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="aaa5d-109">For more information, see:</span></span>

[<span data-ttu-id="aaa5d-110">Microsoft Defender for Endpoint Service에서 장치 오프보딩</span><span class="sxs-lookup"><span data-stu-id="aaa5d-110">Offboard devices from the Microsoft Defender for Endpoint service</span></span>](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[<span data-ttu-id="aaa5d-111">위협 및 취약성 관리의 노출 점수</span><span class="sxs-lookup"><span data-stu-id="aaa5d-111">Exposure score in threat and vulnerability management</span></span>](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[<span data-ttu-id="aaa5d-112">Endpoint용 Microsoft Defender에서 불안정한 센서 수정</span><span class="sxs-lookup"><span data-stu-id="aaa5d-112">Fix unhealthy sensors in Microsoft Defender for Endpoint</span></span>](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[<span data-ttu-id="aaa5d-113">태그 지정을 효과적으로 사용하는 방법(1부)</span><span class="sxs-lookup"><span data-stu-id="aaa5d-113">How to use tagging effectively (Part 1)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[<span data-ttu-id="aaa5d-114">태그 지정을 효과적으로 사용하는 방법(2부)</span><span class="sxs-lookup"><span data-stu-id="aaa5d-114">How to use tagging effectively (Part 2)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[<span data-ttu-id="aaa5d-115">태그 지정을 효과적으로 사용하는 방법(3부)</span><span class="sxs-lookup"><span data-stu-id="aaa5d-115">How to use tagging effectively (Part 3)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




