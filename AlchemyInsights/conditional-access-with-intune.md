---
title: Intune을 사용한 조건부 액세스
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931442"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="ea9d3-102">Intune을 사용한 조건부 액세스</span><span class="sxs-lookup"><span data-stu-id="ea9d3-102">Conditional Access with Intune</span></span>

<span data-ttu-id="ea9d3-103">Intune을 사용 하 여 **조건부 액세스** 를 사용 하려면 3 단계가 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="ea9d3-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="ea9d3-104">장치가 호환 되는 것으로 간주 되기 전에 충족 해야 하는 설정을 정의 하는 **준수 정책** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows))을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="ea9d3-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="ea9d3-105">예를 들어 장치에는 호환 되는 것으로 간주 되기 전에 6 자리 이상의 pin이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ea9d3-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="ea9d3-106">보호할 리소스와 해당 리소스에 액세스 하기 위해 충족 해야 하는 조건을 정의 하는 **조건부 액세스 정책을** 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="ea9d3-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="ea9d3-107">[예를 들어](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) 회사 전자 메일에 액세스 하기 전에 장치가 규격 이어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ea9d3-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="ea9d3-108">**준수 정책과** **조건부 액세스 정책이** 모두 원하는 사용자 그룹을 대상으로 하는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="ea9d3-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="ea9d3-109">이를 위해서는 Azure Active Directory에서 특정 사용자 그룹을 만들어야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ea9d3-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="ea9d3-110">**유용한 링크:**</span><span class="sxs-lookup"><span data-stu-id="ea9d3-110">**Helpful links:**</span></span>

[<span data-ttu-id="ea9d3-111">장치 준수 개요</span><span class="sxs-lookup"><span data-stu-id="ea9d3-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="ea9d3-112">CA 문제 해결</span><span class="sxs-lookup"><span data-stu-id="ea9d3-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="ea9d3-113">문제 해결 정책</span><span class="sxs-lookup"><span data-stu-id="ea9d3-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="ea9d3-114">비규격 장치에서 전자 메일 (Exchange online)을 액세스 하지 못하도록 보호 하려면 두 문서를 모두 준수 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="ea9d3-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="ea9d3-115">EAS를 사용 하 여 장치에서 전자 메일 액세스 보호</span><span class="sxs-lookup"><span data-stu-id="ea9d3-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="ea9d3-116">Outlook과 같은 최신 인증 클라이언트를 사용 하 여 장치에서 전자 메일 액세스 보호</span><span class="sxs-lookup"><span data-stu-id="ea9d3-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)