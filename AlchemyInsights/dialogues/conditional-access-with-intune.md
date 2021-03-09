---
title: Intune에서 조건부 액세스 사용
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529363"
---
# <a name="using-conditional-access-with-intune"></a><span data-ttu-id="5ed92-102">Intune에서 조건부 액세스 사용</span><span class="sxs-lookup"><span data-stu-id="5ed92-102">Using Conditional Access with Intune</span></span>

<span data-ttu-id="5ed92-103">Intune에서 조건부 액세스를 사용하려면 다음 3단계가 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="5ed92-103">Using Conditional Access with Intune requires 3 steps:</span></span>

- [<span data-ttu-id="5ed92-104">준수 정책을 만들어 장치가 규격으로 간주되기 전에 충족해야 하는 설정을 정의합니다. 예를 들어 장치에는 규정 준수로 간주되기 전에 최소 6자리의 핀이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5ed92-104">Create a Compliance Policy to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [<span data-ttu-id="5ed92-105">보호되는 리소스와 해당 리소스에 액세스하기 위해 충족해야 하는 조건을 정의하는 조건부 액세스 정책을 만들 수 있습니다. 예를 들어 회사 전자 메일에 액세스하기 전에 장치를 준수해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="5ed92-105">Create a Conditional Access Policy that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span>](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [<span data-ttu-id="5ed92-106">준수 정책과 조건부 액세스 정책이 모두 원하는 사용자 그룹을 대상으로 하는지 확인 Azure Active Directory에서 특정 사용자 그룹을 만들어야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5ed92-106">Ensure both Compliance Policies and Conditional Access Policies are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[<span data-ttu-id="5ed92-107">자세한 정보...</span><span class="sxs-lookup"><span data-stu-id="5ed92-107">Read more...</span></span>](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
