---
title: 디바이스 태그 또는 그룹 만들기 및 관리
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/02/2021
ms.locfileid: "52721729"
---
# <a name="create-and-manage-device-tags-or-groups"></a><span data-ttu-id="c9923-102">디바이스 태그 또는 그룹 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="c9923-102">Create and manage device tags or groups</span></span>

<span data-ttu-id="c9923-103">디바이스에 태그를 추가하여 논리적 그룹 소속을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="c9923-103">Add tags on devices to create a logical group affiliation.</span></span> <span data-ttu-id="c9923-104">디바이스 태그는 네트워크의 적절한 매핑을 지원하므로 다양한 태그를 연결하여 컨텍스트를 캡처하고 인시던트 일부로 동적 목록 만들기를 사용하도록 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c9923-104">Device tags support proper mapping of the network, enabling you to attach different tags to capture context and to enable dynamic list creation as part of an incident.</span></span> <span data-ttu-id="c9923-105">태그는 디바이스 목록 보기에서 필터로 사용하거나 디바이스를 그룹화하는 데 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c9923-105">Tags can be used as a filter in Devices list view, or to group devices.</span></span> <span data-ttu-id="c9923-106">디바이스 그룹화에 대한 자세한 내용은 [디바이스 태그 만들기 및 관리를](/microsoft-365/security/defender-endpoint/machine-tags) 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c9923-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>

<span data-ttu-id="c9923-107">다음을 수행하여 디바이스에 태그를 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c9923-107">You can add tags on devices by:</span></span>

- <span data-ttu-id="c9923-108">포털 사용</span><span class="sxs-lookup"><span data-stu-id="c9923-108">Using the portal</span></span>

- <span data-ttu-id="c9923-109">레지스트리 키 값 설정</span><span class="sxs-lookup"><span data-stu-id="c9923-109">Setting a registry key value</span></span>
 
<span data-ttu-id="c9923-110">**참고:** 태그가 디바이스에 추가되는 시간과 디바이스 목록 및 디바이스 페이지의 가용성 사이에 대기 시간이 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c9923-110">**Note:** There could be latency between the time a tag is added to a device and its availability in the devices list and device page.</span></span>

<span data-ttu-id="c9923-111">API를 사용하여 디바이스 태그를 추가하려면 [디바이스 태그 API 추가 또는 제거](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c9923-111">To add device tags using API, see [Add or remove device tags API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span></span>

## <a name="add-and-manage-device-tags-using-the-portal"></a><span data-ttu-id="c9923-112">포털을 사용하여 디바이스 태그 추가 및 관리</span><span class="sxs-lookup"><span data-stu-id="c9923-112">Add and manage device tags using the portal</span></span>

1. <span data-ttu-id="c9923-113">태그를 관리할 디바이스를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="c9923-113">Select the device that you want to manage tags on.</span></span> <span data-ttu-id="c9923-114">다음 보기 중 하나에서 디바이스를 선택하거나 검색할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c9923-114">You can select or search for a device from any of the following views:</span></span>

    - <span data-ttu-id="c9923-115">**보안 작업 대시보드** 활성 경고가 있는 상위 디바이스에서 디바이스 이름을 선택하세요.</span><span class="sxs-lookup"><span data-stu-id="c9923-115">**Security operations dashboard** Select the device name from the Top devices with active alerts section.</span></span>
    - <span data-ttu-id="c9923-116">**경고 큐** - 경고 큐에서 디바이스 아이콘 옆에 있는 디바이스 이름을 선택하세요.</span><span class="sxs-lookup"><span data-stu-id="c9923-116">**Alerts queue** - Select the device name beside the device icon from the alerts queue.</span></span>
    - <span data-ttu-id="c9923-117">**디바이스 목록** - 디바이스 목록에서 디바이스 이름을 선택하세요.</span><span class="sxs-lookup"><span data-stu-id="c9923-117">**Devices list** - Select the device name from the list of devices.</span></span>
    - <span data-ttu-id="c9923-118">**검색 상자** - 드롭다운 메뉴에서 디바이스를 선택하고 디바이스 이름을 입력하세요.</span><span class="sxs-lookup"><span data-stu-id="c9923-118">**Search box** - Select Device from the drop-down menu and enter the device name.</span></span>

    <span data-ttu-id="c9923-119">파일 및 IP 보기를 통해 경고 페이지로 이동할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c9923-119">You can also get to the alert page through the file and IP views.</span></span>

1. <span data-ttu-id="c9923-120">응답 작업 행에서 **태그 관리** 를 선택하세요.</span><span class="sxs-lookup"><span data-stu-id="c9923-120">Select **Manage Tags** from the row of Response actions.</span></span>

1. <span data-ttu-id="c9923-121">찾거나 만드려는 태그 입력</span><span class="sxs-lookup"><span data-stu-id="c9923-121">Type to find or create tags.</span></span>

<span data-ttu-id="c9923-122">태그는 디바이스 보기에 추가되고 디바이스 목록 보기에 반영됩니다.</span><span class="sxs-lookup"><span data-stu-id="c9923-122">Tags are added to the device view and are reflected on the Devices list view.</span></span> <span data-ttu-id="c9923-123">그런 다음에는 태그 필터를 사용하여 관련 디바이스 목록을 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c9923-123">You can then use the Tags filter to see the relevant list of devices.</span></span>

<span data-ttu-id="c9923-124">자세한 내용은 [디바이스 태그 만들기 및 관리](/microsoft-365/security/defender-endpoint/machine-tags)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c9923-124">For more information, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>