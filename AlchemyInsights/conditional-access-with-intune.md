---
title: Intune을 통해 조건부 액세스
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704792"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="d1a03-102">Intune을 통해 조건부 액세스</span><span class="sxs-lookup"><span data-stu-id="d1a03-102">Conditional Access with Intune</span></span>

<span data-ttu-id="d1a03-103">Intune에서  **조건부**  액세스를 사용하려면 다음 3단계가 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="d1a03-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="d1a03-104">준수  [정책(Android,](https://docs.microsoft.com/intune/compliance-policy-create-android) [iOS,](https://docs.microsoft.com/intune/compliance-policy-create-ios) [Windows)을](https://docs.microsoft.com//intune/compliance-policy-create-windows)만들어 장치가 규격으로 간주되기 전에 충족해야 하는 설정을 정의합니다.</span><span class="sxs-lookup"><span data-stu-id="d1a03-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="d1a03-105">예를 들어 장치에는 규정 준수로 간주되기 전에 최소 6자리의 핀이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="d1a03-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="d1a03-106">보호되는 리소스와 해당 **리소스에 액세스하기**  위해 충족해야 하는 조건을 정의하는 조건부 액세스 정책을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d1a03-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="d1a03-107">[예를 들어 회사](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  전자 메일에 액세스하기 전에 장치를 준수해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="d1a03-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="d1a03-108">준수 **정책과**  **조건부 액세스**  정책이 모두 원하는 사용자 그룹을 대상으로 하는지 확인</span><span class="sxs-lookup"><span data-stu-id="d1a03-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="d1a03-109">Azure Active Directory에서 특정 사용자 그룹을 만들어야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d1a03-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="d1a03-110">**유용한 링크:**</span><span class="sxs-lookup"><span data-stu-id="d1a03-110">**Helpful links:**</span></span>

[<span data-ttu-id="d1a03-111">장치 준수 개요</span><span class="sxs-lookup"><span data-stu-id="d1a03-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="d1a03-112">CA 문제 해결</span><span class="sxs-lookup"><span data-stu-id="d1a03-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="d1a03-113">문제 해결 정책</span><span class="sxs-lookup"><span data-stu-id="d1a03-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="d1a03-114">비호환 장치의 액세스로부터 전자 메일(Exchange Online)을 보호하려면 두 문서를 모두 따라야 합니다.</span><span class="sxs-lookup"><span data-stu-id="d1a03-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="d1a03-115">EAS를 사용하여 장치에서 전자 메일 액세스 보호</span><span class="sxs-lookup"><span data-stu-id="d1a03-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="d1a03-116">Outlook과 같은 최신 인증 클라이언트를 사용하여 장치에서 전자 메일 액세스 보호</span><span class="sxs-lookup"><span data-stu-id="d1a03-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)