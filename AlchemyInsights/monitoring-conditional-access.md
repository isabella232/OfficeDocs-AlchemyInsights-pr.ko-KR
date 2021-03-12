---
title: 조건부 액세스 모니터링
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708680"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="38d24-102">Exchange에 대한 조건부 액세스 모니터링</span><span class="sxs-lookup"><span data-stu-id="38d24-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="38d24-103">조건부 액세스를 대상으로 하는 사용자는 조직의 액세스 요구 사항을 충족하지 않는 경우 알림 전자 메일을 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="38d24-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="38d24-104">해결을 위해 다음 솔루션 중 하나 이상을 해결하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="38d24-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="38d24-105">디바이스가 등록된 것으로 확인된 경우 사용자에게 회사 포털 앱으로 이동하여 회사 포털에 나타나는지 확인하도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="38d24-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="38d24-106">그렇지 않은 경우 사용자는 장치를 등록해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="38d24-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="38d24-107">Azure Portal에서 Intune > 장치 준수로 이동하세요.</span><span class="sxs-lookup"><span data-stu-id="38d24-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="38d24-108">모니터에서 장치 준수를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="38d24-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="38d24-109">장치 준수 보고서를 보고 사용자의 장치가 규격으로 표시되어 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="38d24-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="38d24-110">Azure Portal에서 Intune > 장치 준수로 이동하세요.</span><span class="sxs-lookup"><span data-stu-id="38d24-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="38d24-111">관리에서 정책을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="38d24-111">Under Manage, click Policies.</span></span> <span data-ttu-id="38d24-112">준수 정책 목록에서 프로필이 사용자의 장치에 할당되어 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="38d24-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="38d24-113">프로필이 할당되지 않은 경우 Intune에서 장치의 준수 상태를 확인할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="38d24-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="38d24-114">사용자의 조건부 액세스 할당을 편집합니다.</span><span class="sxs-lookup"><span data-stu-id="38d24-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="38d24-115">Azure Portal에서 **Intune**  >  **조건부 액세스 정책으로**  >  **이동하세요.**</span><span class="sxs-lookup"><span data-stu-id="38d24-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="38d24-116">목록에서 정책을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="38d24-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="38d24-117">사용자 및 그룹을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="38d24-117">Click Users and groups.</span></span>
4. <span data-ttu-id="38d24-118">누군가의 특정 정책을 대상으로 지정하기 위해 포함 목록에 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="38d24-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="38d24-119">사용자가 정책에서 생략되도록 제외 목록에 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="38d24-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="38d24-120">유용한 링크:</span><span class="sxs-lookup"><span data-stu-id="38d24-120">Helpful links:</span></span>

[<span data-ttu-id="38d24-121">장치 준수 개요</span><span class="sxs-lookup"><span data-stu-id="38d24-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="38d24-122">CA 문제 해결</span><span class="sxs-lookup"><span data-stu-id="38d24-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="38d24-123">문제 해결 정책</span><span class="sxs-lookup"><span data-stu-id="38d24-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="38d24-124">Intune 장치 준수 모니터링</span><span class="sxs-lookup"><span data-stu-id="38d24-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="38d24-125">참고: 이러한 단계는 Azure Active Directory 기능 조건부 액세스를 해결하는 데에만 유용합니다.</span><span class="sxs-lookup"><span data-stu-id="38d24-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="38d24-126">또한 Exchange 정책을 사용하여 전자 메일 액세스를 차단하는 장치를 차단할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="38d24-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="38d24-127">Exchange 장치 관리에 대한 자세한 내용은 [here]( 를 https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) 참조하십시오.</span><span class="sxs-lookup"><span data-stu-id="38d24-127">More information on Exchange device management can be found [here](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141).</span></span>
