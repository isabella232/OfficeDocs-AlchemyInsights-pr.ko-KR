---
title: Intune을 사용하여 분실된 iOS 장치 찾기
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434596"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="1e26c-102">Intune을 사용하여 분실된 iOS 장치 찾기</span><span class="sxs-lookup"><span data-stu-id="1e26c-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="1e26c-103">iOS 장치에서 분실 모드를 사용하도록 설정하면 관리자가 잠금 화면에 메시지와 연락처 전화 번호를 표시할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1e26c-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="1e26c-104">분실 모드를 사용하도록 설정한 후 관리자가 장치 찾기 작업을 사용하여 장치의 실제 위치를 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1e26c-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="1e26c-105">Intune의 장치 찾기 작업은 iOS 장치에서 작동하여 지도에서 특정 장치의 위치를 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="1e26c-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="1e26c-106">이 작업을 사용하려면 iOS 장치에서 다음을 사용해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e26c-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="1e26c-107">감독 모드</span><span class="sxs-lookup"><span data-stu-id="1e26c-107">Supervised mode</span></span>
- <span data-ttu-id="1e26c-108">분실 모드</span><span class="sxs-lookup"><span data-stu-id="1e26c-108">Lost mode</span></span>

<span data-ttu-id="1e26c-109">자세한 내용은 [Intune을 사용하여 iOS/iPadOS 장치에서 분실 모드 사용](https://docs.microsoft.com/intune/device-lost-mode) 및 [Intune을 사용하여 분실하거나 도난당한 iOS/iPadOS 장치 찾기](https://docs.microsoft.com/intune/device-locate)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1e26c-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="1e26c-110">**FAQ**</span><span class="sxs-lookup"><span data-stu-id="1e26c-110">**FAQ**</span></span>

<span data-ttu-id="1e26c-111">Q: 장치에서 회사 데이터를 제거하기 위한 원격 작업을 실행했는데, 현재 계속 보류 상태입니다.</span><span class="sxs-lookup"><span data-stu-id="1e26c-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="1e26c-112">A: 원격 작업이 성공적으로 완료되려면 대상 장치가 온라인 상태여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e26c-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="1e26c-113">다음과 같은 경우 원격 작업은 30일 동안 또는 장치가 명령을 인식할 때까지 보류 상태로 유지됩니다.</span><span class="sxs-lookup"><span data-stu-id="1e26c-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="1e26c-114">장치에 연결할 수 없는 경우</span><span class="sxs-lookup"><span data-stu-id="1e26c-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="1e26c-115">장치가 Intune에서 관리 상태가 누락되는 경우</span><span class="sxs-lookup"><span data-stu-id="1e26c-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="1e26c-116">장치가 더 이상 체크인하지 않고 회사 데이터를 제거할 수 없는 경우, 삭제를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="1e26c-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="1e26c-117">삭제하면 장치 레코드가 제거되어 장치의 Intune 목록에 더 이상 나타나지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1e26c-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="1e26c-118">장치가 다시 활성화되면 사용자가 이를 다시 등록해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="1e26c-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="1e26c-119">Q: 특정 원격 작업을 사용할 수 없는 이유는 무엇입니까?</span><span class="sxs-lookup"><span data-stu-id="1e26c-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="1e26c-120">A: 모든 플랫폼이 모든 원격 장치 작업을 지원하는 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="1e26c-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="1e26c-121">다음 원격 작업은 플랫폼에 따라 달라지며 언급된 플랫폼에서만 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1e26c-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="1e26c-122">활성화 잠금을 바이패스합니다(iOS만 해당).</span><span class="sxs-lookup"><span data-stu-id="1e26c-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="1e26c-123">새로 시작합니다(Windows 전용).</span><span class="sxs-lookup"><span data-stu-id="1e26c-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="1e26c-124">모드가 손실되었습니다(iOS만 해당).</span><span class="sxs-lookup"><span data-stu-id="1e26c-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="1e26c-125">장치를 찾습니다(iOS만 해당).</span><span class="sxs-lookup"><span data-stu-id="1e26c-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="1e26c-126">다시 시작합니다(Windows 전용).</span><span class="sxs-lookup"><span data-stu-id="1e26c-126">Restart (Windows only)</span></span>

<span data-ttu-id="1e26c-127">각 작업에 대한 자세한 내용은 [사용 가능한 디바이스 작업](https://docs.microsoft.com/intune/device-management#available-device-actions)을(를) 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="1e26c-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>