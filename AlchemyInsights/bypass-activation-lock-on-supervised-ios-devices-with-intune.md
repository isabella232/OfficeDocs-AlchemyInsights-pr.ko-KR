---
title: Intune으로 감독되는 iOS 기기에서 활성화 잠금 우회
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 743b5917c08b0a49a8c5791bdeb59a1672dd0fc7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757306"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a><span data-ttu-id="7e87b-102">Intune으로 감독되는 iOS 기기에서 활성화 잠금 우회</span><span class="sxs-lookup"><span data-stu-id="7e87b-102">Bypass activation lock on supervised iOS devices with Intune</span></span>

<span data-ttu-id="7e87b-103">iOS 기기의 정품 인증 잠금을 우회할 수 있으므로 사용자가 회사 기기에서 정품 인증 잠금을 활성화한 다음 회사를 떠나는 시나리오에서 쉽게 복구할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7e87b-103">The ability to bypass the activation lock on iOS devices makes it easier to recover from the scenario where a user enables activation lock on a corporate device, and then leaves the company.</span></span>

<span data-ttu-id="7e87b-104">활성화 잠금을 바이패스하기 위한 사전 요구사항은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="7e87b-104">Pre-requisites to bypassing an activation lock include:</span></span>

- <span data-ttu-id="7e87b-105">장치는 "감독된" 장치입니다."</span><span class="sxs-lookup"><span data-stu-id="7e87b-105">A device is that is "supervised."</span></span>
- <span data-ttu-id="7e87b-106">Intune에서 iOS 장치 제한 정책을 사용하여 활성화 잠금을 성공적으로 활성화했습니다.</span><span class="sxs-lookup"><span data-stu-id="7e87b-106">The activation lock is successfully enabled using iOS Device restriction policy in Intune.</span></span>

<span data-ttu-id="7e87b-107">또한 활성화 잠금을 바이패스할 때는 다음을 수행해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="7e87b-107">In addition, when bypassing an activation lock, you should:</span></span>

- <span data-ttu-id="7e87b-108">지우는 장치를 물리적으로 소유합니다.</span><span class="sxs-lookup"><span data-stu-id="7e87b-108">Physically possess the device being wiped.</span></span>
- <span data-ttu-id="7e87b-109">지우기 전에 코드를 복사합니다.</span><span class="sxs-lookup"><span data-stu-id="7e87b-109">Copy the code before you issue the wipe.</span></span>

<span data-ttu-id="7e87b-110">**참고:** 지우기 코드는 대소문자를 구분하지 않으므로 "-" 문자는 필요하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="7e87b-110">**Note:** The wipe code is not case sensitive, so the "-" characters are not required.</span></span>

<span data-ttu-id="7e87b-111">자세한 내용은 [Intune에서 감독되는 iOS 디바이스에 대한 정품 인증 잠금 바이패스(Bypass)](https://docs.microsoft.com/intune/device-activation-lock-bypass)를 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="7e87b-111">For details, see [Bypass Activation Lock on Supervised iOS devices with Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span></span>

<span data-ttu-id="7e87b-112">**FAQ**</span><span class="sxs-lookup"><span data-stu-id="7e87b-112">**FAQ**</span></span>

<span data-ttu-id="7e87b-113">Q: **장치에서 회사 데이터를 제거하기 위한 원격 작업을 실행했는데, 현재 보류 상태에 빠졌습니다.**</span><span class="sxs-lookup"><span data-stu-id="7e87b-113">Q: **I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.**</span></span>

<span data-ttu-id="7e87b-114">A: 원격 작업이 성공적으로 완료되려면 대상 장치가 온라인 상태여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="7e87b-114">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="7e87b-115">다음과 같은 경우 원격 작업은 30일 동안 또는 장치가 명령을 인식할 때까지 보류 상태로 유지됩니다.</span><span class="sxs-lookup"><span data-stu-id="7e87b-115">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command when the device:</span></span>

- <span data-ttu-id="7e87b-116">연결이 없습니다.</span><span class="sxs-lookup"><span data-stu-id="7e87b-116">Does not have connectivity.</span></span>
- <span data-ttu-id="7e87b-117">Intune에서 관리 상태를 손실합니다.</span><span class="sxs-lookup"><span data-stu-id="7e87b-117">Loses its management status with Intune.</span></span>

<span data-ttu-id="7e87b-118">장치가 더 이상 체크인하지 않고 회사 데이터를 제거하지 않을 경우 삭제를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="7e87b-118">If you think a device is no longer checking in, and that it won’t remove company data, select Delete.</span></span> <span data-ttu-id="7e87b-119">삭제하면 장치 레코드가 제거되어 장치의 Intune 목록에 더 이상 나타나지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="7e87b-119">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="7e87b-120">장치를 다시 활성화하려면 사용자가 장치를 다시 등록해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="7e87b-120">For the device to become active again, its user must re-enroll the device.</span></span>

<span data-ttu-id="7e87b-121">Q: **특정 원격 작업을 사용할 수 없는 이유는 무엇입니까?**</span><span class="sxs-lookup"><span data-stu-id="7e87b-121">Q: **Why are certain remote actions not available for me to use?**</span></span>

<span data-ttu-id="7e87b-122">A: 모든 플랫폼이 모든 원격 장치 작업을 지원하는 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="7e87b-122">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="7e87b-123">다음 원격 작업은 플랫폼별로 다릅니다.</span><span class="sxs-lookup"><span data-stu-id="7e87b-123">The following remote actions are platform-specific.</span></span>

- <span data-ttu-id="7e87b-124">활성화 잠금을 바이패스합니다(iOS만 해당).</span><span class="sxs-lookup"><span data-stu-id="7e87b-124">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="7e87b-125">새로 시작합니다(Windows 전용).</span><span class="sxs-lookup"><span data-stu-id="7e87b-125">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="7e87b-126">모드가 손실되었습니다(iOS만 해당).</span><span class="sxs-lookup"><span data-stu-id="7e87b-126">Lost mode (iOS only)</span></span>
- <span data-ttu-id="7e87b-127">장치를 찾습니다(iOS만 해당).</span><span class="sxs-lookup"><span data-stu-id="7e87b-127">Locate device (iOS only)</span></span>
- <span data-ttu-id="7e87b-128">다시 시작합니다(Windows 전용).</span><span class="sxs-lookup"><span data-stu-id="7e87b-128">Restart (Windows only)</span></span>

<span data-ttu-id="7e87b-129">각 작업에 대한 자세한 내용은 [사용 가능한 디바이스 작업](https://docs.microsoft.com/intune/device-management#available-device-actions)을(를) 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="7e87b-129">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>