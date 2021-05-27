---
title: 소프트웨어 인벤터리가 없거나 부정확 합니다.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52658053"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a><span data-ttu-id="cd8a8-102">소프트웨어 인벤터리가 없거나 부정확 합니다.</span><span class="sxs-lookup"><span data-stu-id="cd8a8-102">Software inventory is missing or inaccurate</span></span>

<span data-ttu-id="cd8a8-103">위협 및 TVM(취약성 관리)의 소프트웨어 인벤토리는 공식 CPE(공통 플랫폼 열거)가 있는 조직의 알려진 소프트웨어 목록입니다.</span><span class="sxs-lookup"><span data-stu-id="cd8a8-103">The software inventory in threat and vulnerability management (TVM) is a list of known software in your organization with official Common Platform Enumerations (CPE).</span></span>

<span data-ttu-id="cd8a8-104">공식 CPE가 없는 소프트웨어 제품에는 취약성이 게시되지 않았습니다.</span><span class="sxs-lookup"><span data-stu-id="cd8a8-104">Software products without an official CPE don’t have vulnerabilities published.</span></span> <span data-ttu-id="cd8a8-105">인벤토리에는 공급업체 이름, 취약점 수, 위협 및 노출된 장치 수와 같은 세부 정보도 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="cd8a8-105">The inventory also includes details such as the name of the vendor, number of weaknesses, threats, and number of exposed devices.</span></span>

<span data-ttu-id="cd8a8-106">장치의 소프트웨어 변경 사항은 일반적으로 보안 포털에 2시간 이내에 반영됩니다.</span><span class="sxs-lookup"><span data-stu-id="cd8a8-106">Software changes on devices are typically reflected in security portals within two hours.</span></span> <span data-ttu-id="cd8a8-107">하지만, 때때로 더 오래 걸릴 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cd8a8-107">However, it may sometimes take longer.</span></span> <span data-ttu-id="cd8a8-108">현재 동기화를 강제할 수 있는 방법은 없습니다. 지속적인 평가입니다.</span><span class="sxs-lookup"><span data-stu-id="cd8a8-108">There’s currently no way to force a sync; this is an ongoing continuous assessment.</span></span>

<span data-ttu-id="cd8a8-109">소프트웨어를 변경했는데 5시간 후에 변경 사항이 TVM에 정확하게 반영되지 않는 경우 다음 단계를 수행하세요.</span><span class="sxs-lookup"><span data-stu-id="cd8a8-109">If you made a software change and the change is not accurately reflected in TVM after 5 hours, follow these steps:</span></span>

1. <span data-ttu-id="cd8a8-110">소프트웨어 증거 섹션을 확인하여 소프트웨어가 어떻게 감지되었는지 알아보세요.</span><span class="sxs-lookup"><span data-stu-id="cd8a8-110">Check the software evidence section to understand how the software was detected.</span></span>
1. <span data-ttu-id="cd8a8-111">소프트웨어가 지원되는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="cd8a8-111">Make sure that the software is supported.</span></span> <span data-ttu-id="cd8a8-112">소프트웨어는 현재 위협 및 취약성 관리에서 지원되지 않는 경우에도 장치 수준에서만 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cd8a8-112">Software may be visible only at the device level even if it is currently not supported by threat and vulnerability management.</span></span> <span data-ttu-id="cd8a8-113">그러나 제한된 데이터만 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cd8a8-113">However, only limited data is available.</span></span>
1. <span data-ttu-id="cd8a8-114">포털에서 부정확성을 보고하는 단계는 [부정확성 보고](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd8a8-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span></span>
   
    <span data-ttu-id="cd8a8-115">**참고**: MDE 포털에서 부정확성을 보고하는 것은 엔지니어링을 위한 단방향 채널입니다.</span><span class="sxs-lookup"><span data-stu-id="cd8a8-115">**Note**: Reporting an inaccuracy from the MDE portal is a one-way channel to engineering.</span></span> <span data-ttu-id="cd8a8-116">문제가 긴급하면 지원 티켓을 여세요.</span><span class="sxs-lookup"><span data-stu-id="cd8a8-116">If the issue is urgent, open a support ticket.</span></span>

<span data-ttu-id="cd8a8-117">더 자세한 내용은 [소프트웨어 인벤토리 - 위협 및 취약성 관리](/microsoft-365/security/defender-endpoint/tvm-software-inventory)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd8a8-117">For more information, see [Software inventory - threat and vulnerability management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span></span>