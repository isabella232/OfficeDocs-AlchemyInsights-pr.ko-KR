---
title: Intune 조건부 액세스 모니터링
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/03/2021
ms.locfileid: "50417318"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="edb2b-102">Intune 조건부 액세스 모니터링</span><span class="sxs-lookup"><span data-stu-id="edb2b-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="edb2b-103">조건부 액세스를 대상으로 하는 사용자는 조직의 액세스 요구 사항을 충족하지 않는 경우 알림 전자 메일을 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="edb2b-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="edb2b-104">해결을 위해 다음 솔루션 중 하나 이상을 해결하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="edb2b-104">To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="edb2b-105">디바이스가 등록된 것으로 확인된 경우 사용자에게 회사 포털 앱으로 이동하여 회사 포털에 나타나는지 확인하도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="edb2b-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="edb2b-106">그렇지 않은 경우 사용자는 장치를 등록해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="edb2b-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="edb2b-107">Azure Portal에서 **Intune 장치**  >  **준수로 이동하세요.**</span><span class="sxs-lookup"><span data-stu-id="edb2b-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="edb2b-108">장치 준수 보고서를 보고 사용자의 장치가 규격으로 표시되어 있는지 확인하려면 모니터링에서 장치 준수 **를 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="edb2b-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="edb2b-109">Azure Portal에서 **Intune 장치**  >  **준수로 이동하세요.**</span><span class="sxs-lookup"><span data-stu-id="edb2b-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="edb2b-110">관리에서 **정책을** **클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="edb2b-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="edb2b-111">준수 정책 목록에서 프로필이 사용자의 장치에 할당되어 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="edb2b-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="edb2b-112">프로필이 할당되지 않은 경우 Intune에서 장치의 준수 상태를 확인할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="edb2b-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="edb2b-113">사용자의 조건부 액세스 할당을 편집합니다.</span><span class="sxs-lookup"><span data-stu-id="edb2b-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="edb2b-114">Azure Portal에서 **Intune**  >  **조건부 액세스** 정책으로 이동하여 목록에서 정책을 선택하고 사용자 및 그룹을  >   **클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="edb2b-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="edb2b-115">누군가의 특정 정책을 대상으로 지정하기 위해 포함 목록에 **추가합니다.**</span><span class="sxs-lookup"><span data-stu-id="edb2b-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="edb2b-116">사용자가 정책에서 생략되도록 제외 목록에 **추가합니다.**</span><span class="sxs-lookup"><span data-stu-id="edb2b-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="edb2b-117">**유용한 링크:**</span><span class="sxs-lookup"><span data-stu-id="edb2b-117">**Helpful links:**</span></span>

- [<span data-ttu-id="edb2b-118">장치 준수 개요</span><span class="sxs-lookup"><span data-stu-id="edb2b-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="edb2b-119">CA 문제 해결</span><span class="sxs-lookup"><span data-stu-id="edb2b-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="edb2b-120">문제 해결 정책</span><span class="sxs-lookup"><span data-stu-id="edb2b-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="edb2b-121">Intune 장치 준수 모니터링</span><span class="sxs-lookup"><span data-stu-id="edb2b-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="edb2b-122">이러한 단계는 Azure Active Directory 기능 조건부 액세스를 해결하는 데에만 유용합니다.</span><span class="sxs-lookup"><span data-stu-id="edb2b-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="edb2b-123">또한 Exchange 정책을 사용하여 전자 메일 액세스를 차단하는 장치를 차단할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="edb2b-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="edb2b-124">Exchange 장치 관리에 대한 자세한 내용은 에서 찾을 수 [**있습니다.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))</span><span class="sxs-lookup"><span data-stu-id="edb2b-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
