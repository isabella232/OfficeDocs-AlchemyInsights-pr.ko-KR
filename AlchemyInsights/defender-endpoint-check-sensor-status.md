---
title: Defender 엔드포인트 확인 센서 상태
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/24/2021
ms.locfileid: "52627243"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="367c3-102">Defender 엔드포인트 확인 센서 상태</span><span class="sxs-lookup"><span data-stu-id="367c3-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="367c3-103">**센서 문제가 있는 장치** 타일이 보안 작업 대시보드에 있습니다.</span><span class="sxs-lookup"><span data-stu-id="367c3-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="367c3-104">이 타일은 개별 장치에서 센서 데이터를 제공하고 엔드포인트용 Defender 서비스와 통신하는 기능의 정보를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="367c3-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="367c3-105">주의가 필요한 장치 수를 보고하고 문제가 있는 장치를 식별하고 알려진 문제를 수정하기 위한 조치를 취하는 데 도움이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="367c3-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="367c3-106">타일의 두 상태 표시기는 서비스에 제대로 보고하지 않는 장치 수에 대한 정보를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="367c3-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="367c3-107">부분적으로 엔드포인트용 Defender 서비스에 센서 데이터를 보고하고 있을 수 있으며 수정해야 하는 구성 오류가 있을 수 있는 **잘못 구성된** 장치입니다.</span><span class="sxs-lookup"><span data-stu-id="367c3-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="367c3-108">지난 달에 7일 이상 엔드포인트용 Defender 서비스에 보고를 중지한 **대화 불가능** 장치입니다.</span><span class="sxs-lookup"><span data-stu-id="367c3-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="367c3-109">그룹을 클릭하면 선택에 따라 필터링된 장치 목록으로 연결됩니다.</span><span class="sxs-lookup"><span data-stu-id="367c3-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="367c3-110">장치 목록에서 다음 상태로 상태 목록을 필터링할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="367c3-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="367c3-111">엔드포인트용 Defender 서비스에 활발히 보고하고 있는 **대화 가능** 장치입니다.</span><span class="sxs-lookup"><span data-stu-id="367c3-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="367c3-112">부분적으로 엔드포인트용 Defender 서비스에 센서 데이터를 보고하고 있을 수 있으나 수정해야 하는 구성 오류가 있는 **잘못 구성된** 장치입니다.</span><span class="sxs-lookup"><span data-stu-id="367c3-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="367c3-113">잘못 구성된 장치에는 다음 문제 중 하나 또는 문제의 조합이 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="367c3-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="367c3-114">센서 데이터가 없습니다. 장치가 센서 데이터 전송을 중지했습니다.</span><span class="sxs-lookup"><span data-stu-id="367c3-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="367c3-115">장치에서 제한된 경고를 트리거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="367c3-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="367c3-116">통신 장애 - 장치와 통신하는 기능에 장애가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="367c3-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="367c3-117">심층 분석을 위한 파일 전송, 파일 차단, 네트워크에서 장치 분리, 장치와 통신이 필요한 기타 작업이 작동하지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="367c3-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="367c3-118">엔드포인트용 Defender 서비스에 보고를 중지한 **대화 불가능** 장치입니다.</span><span class="sxs-lookup"><span data-stu-id="367c3-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="367c3-119">내보내기 기능을 사용하여 CSV 형식으로 전체 목록을 다운로드할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="367c3-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="367c3-120">자세한 내용은 [엔드포인트용 Microsoft Defender에서 센서 상태 확인](/microsoft-365/security/defender-endpoint/check-sensor-status)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="367c3-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="367c3-121">장치가 대화가 불가능하게 되거나 잘못 구성된 원인에 대한 자세한 내용은 [엔드포인트용 Microsoft Defender에서 비정상 센서 수정](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="367c3-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
