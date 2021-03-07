---
title: 특성 및 범위 지정 필터에 문제가 있는 경우
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430779"
---
# <a name="problem-with-attribute-and-scoping-filter"></a><span data-ttu-id="9ba38-102">특성 및 범위 지정 필터에 문제가 있는 경우</span><span class="sxs-lookup"><span data-stu-id="9ba38-102">Problem with attribute and scoping filter</span></span>

<span data-ttu-id="9ba38-103">**UPN 값 충돌 문제**</span><span class="sxs-lookup"><span data-stu-id="9ba38-103">**Issue with conflicting UPN values**</span></span>

<span data-ttu-id="9ba38-104">Workday ~ AD 사용자 프로비전 Workday ~ AD 사용자 프로비전 작업 시 **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique** 오류 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="9ba38-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span></span> <span data-ttu-id="9ba38-105">추가/수정을 위해 입력한 UPN 값이 포리스트 범위에서 고유하지 않아서 작업이 실패했습니다.</span><span class="sxs-lookup"><span data-stu-id="9ba38-105">The operation failed because UPN value provided for addition/modification is not unique forest-wide.</span></span> <span data-ttu-id="9ba38-106">오류 세부 정보: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="9ba38-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span></span>

<span data-ttu-id="9ba38-107">AD 사용자 계정을 만들 때 Workday 커넥터에서 설정하려고 하는 **userPrincipalName** 값이 대상 AD 도메인에 이미 존재합니다.</span><span class="sxs-lookup"><span data-stu-id="9ba38-107">The **userPrincipalName** value that Workday connector is trying to set when creating the AD user account already exists in the target AD domain.</span></span> <span data-ttu-id="9ba38-108">즉, (1) 사용자가 이미 존재하며 해당 사용자에 대한 일치하는 ID 검사가 실패했거나 (2) UPN 생성 규칙에 따라 충돌하는 값이 발생한 것입니다.</span><span class="sxs-lookup"><span data-stu-id="9ba38-108">This implies that either (1) the user already exists and the matching ID check failed for the user or (2) the UPN generation rule generated a conflicting value.</span></span>

<span data-ttu-id="9ba38-109">제안된 해결 단계는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="9ba38-109">Here are the suggested resolution steps:</span></span>

<span data-ttu-id="9ba38-110">사용자가 이미 있으며 일치하는 ID 검사에서 Workday 계정을 Active Directory 계정에 연결하지 못한 경우라면 Workday와 AD 양쪽에서 일치하는 ID 특성(일반적으로 **employeeID**)이 정확히 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="9ba38-110">If the user already exists and the matching ID check failed to link the Workday account to Active Directory account, then check if the matching ID attribute (typically **employeeID**) in both Workday and AD have an exact match.</span></span> <span data-ttu-id="9ba38-111">일치하지 않는 경우 수정해야 하는 데이터 문제입니다.</span><span class="sxs-lookup"><span data-stu-id="9ba38-111">If they don't have a match, it is a data issue that needs to be fixed.</span></span> <span data-ttu-id="9ba38-112">예를 들어 Workday의 EmployeeID는 001052이고 AD의 EmployeeID는 1052라면 프로비전 엔진이 두 계정을 연결하지 못하고 이미 존재하는 사용자를 만들려고 합니다.</span><span class="sxs-lookup"><span data-stu-id="9ba38-112">For example, if the EmployeeID in Workday is 001052 and in AD it is 1052, then the provisioning engine will fail to link the two accounts and will try to create a user that already exists.</span></span> <span data-ttu-id="9ba38-113">이 경우의 해결 방법은 AD의 **EmployeeID** 값 앞에 0을 집어넣어 001052로 되도록 변경하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="9ba38-113">The solution in this case is to change the **EmployeeID** value in AD to include the leading zeros to make it 001052.</span></span>
<span data-ttu-id="9ba38-114">UPN 생성 식에서 고유 값을 생성하지 않는 경우 중복 제거 함수 **SelectUniqueValue** 를 사용하여 매번 고유한 값을 생성하게 하는 것이 고려해 보세요.</span><span class="sxs-lookup"><span data-stu-id="9ba38-114">If the UPN-generating expression is not generating a unique value, consider using the de-duplication function **SelectUniqueValue** to generate a unique value each time.</span></span>

<span data-ttu-id="9ba38-115">**Workday ~ AD 사용자 프로비전 작업에서 AD 사용자 계정에 대한 관리자 특성 값이 설정되지 않는 경우**</span><span class="sxs-lookup"><span data-stu-id="9ba38-115">**Workday to AD User Provisioning does not set manager attribute value for AD user account**</span></span>

<span data-ttu-id="9ba38-116">Workday ~ AD 사용자 프로비전 작업에서 AD 사용자 계정에 대한 **관리자** 특성 값을 설정하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="9ba38-116">The Workday to AD User Provisioning job is not setting the **manager** attribute value for AD user accounts.</span></span> <span data-ttu-id="9ba38-117">이러한 동작이 관찰되는 경우 가능한 다음 두 가지 시나리오가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9ba38-117">There are two possible scenarios when this behavior is seen:</span></span>

1. <span data-ttu-id="9ba38-118">관리자는 검색 범위에 포함되지 않아 Workday의 관리자가 해당하는 AD 사용자 계정으로 해결되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="9ba38-118">The manager in Workday cannot be resolved to a corresponding AD User account because the manager is not in scope.</span></span>
2. <span data-ttu-id="9ba38-119">**여러 AD 도메인** 시나리오에서는 Workday의 관리자가 사용자와 동일한 도메인에 있지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="9ba38-119">In a **multiple AD domains** scenario, the manager in Workday is not present in the same domain as the user.</span></span>

<span data-ttu-id="9ba38-120">다음 단계를 시도하여 문제를 해결하세요.</span><span class="sxs-lookup"><span data-stu-id="9ba38-120">Try these steps to resolve the issue:</span></span>

1. <span data-ttu-id="9ba38-121">범위 지정 필터를 정의한 경우 먼저 관리자가 범위 내에 있으며 범위 지정 절을 충족하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="9ba38-121">If you have defined scoping filters, first check if the manager is in scope and that it satisfies the scoping clause.</span></span> <span data-ttu-id="9ba38-122">관리자가 범위 지정 필터를 충족하지 않는 경우 관리자가 프로비전 작업의 범위에 포함되도록 필터를 변경합니다.</span><span class="sxs-lookup"><span data-stu-id="9ba38-122">If the manager does not satisfy the scoping filter, change the filter so that the manager is also in scope of the provisioning operation.</span></span>
2. <span data-ttu-id="9ba38-123">AD 도메인이 여러 개인 경우 커넥터에 도메인 간 관리자 참조를 해결하지 못하는 제한이 있는 것으로 알려졌습니다.</span><span class="sxs-lookup"><span data-stu-id="9ba38-123">If you have multiple AD domains, then the connector has a known limitation of inability to resolve cross-domain manager references.</span></span>

<span data-ttu-id="9ba38-124">자동 프로비전 작업일을 구성하는 방법에 대한 자세한 내용은 [자습서: 자동 사용자 프로비전 작업일 구성](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="9ba38-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>













