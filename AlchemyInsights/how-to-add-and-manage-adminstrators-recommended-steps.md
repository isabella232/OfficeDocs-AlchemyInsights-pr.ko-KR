---
title: 관리자 추가 및 관리 방법 - 권장 단계
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 142bf1474ac0e0eac5cecb9dddd35e28b6b6631e
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599520"
---
# <a name="how-to-add-and-manage-adminstrators---recommended-steps"></a><span data-ttu-id="ef393-102">관리자 추가 및 관리 방법 - 권장 단계</span><span class="sxs-lookup"><span data-stu-id="ef393-102">How to add and manage adminstrators - recommended steps</span></span>

<span data-ttu-id="ef393-103">**구독 관리자 또는 공동 관리자 편집**</span><span class="sxs-lookup"><span data-stu-id="ef393-103">**Edit the Subscription Administrator or Co-administrator**</span></span>

- <span data-ttu-id="ef393-104">계정 관리자는 두 역할을 모두 편집할 수 있는 반면 구독 관리자는 Azure Portal에서 공동 관리자만 변경할 [수 있습니다.](https://ms.portal.azure.com/#home)</span><span class="sxs-lookup"><span data-stu-id="ef393-104">The Account Administrator can edit both roles whereas the Subscription Administrator can only change Co-administrators in the [Azure portal](https://ms.portal.azure.com/#home).</span></span>
- [<span data-ttu-id="ef393-105">Azure 구독 관리자 추가 또는 변경</span><span class="sxs-lookup"><span data-stu-id="ef393-105">Add or change Azure subscription administrators</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

<span data-ttu-id="ef393-106">**내부(AIRS) Co-Administrator 구독 관리자 또는 구독 업데이트**</span><span class="sxs-lookup"><span data-stu-id="ef393-106">**Update the Subscription Administrator or Co-Administrator for Internal (AIRS) Subscriptions**</span></span>

<span data-ttu-id="ef393-107">서비스 관리자 또는 공동 관리자는 다음 단계를 사용하여 이 작업을 셀프 서비스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ef393-107">The Service Administrator or the Co-administrator can self-serve this action by using the following steps:</span></span>

1. <span data-ttu-id="ef393-108">[Azure Portal에 로그인하고](https://ms.portal.azure.com/#home) 왼쪽 블레이드에서 비용 관리 **+** 청구를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="ef393-108">Log in to the [Azure portal](https://ms.portal.azure.com/#home) and click **Cost Management + Billing** in the left blade.</span></span>
2. <span data-ttu-id="ef393-109">구독이 있는 품목을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="ef393-109">Click on the line item with your subscription.</span></span> <span data-ttu-id="ef393-110">그러면 구독에 대한 개요가 열립니다.</span><span class="sxs-lookup"><span data-stu-id="ef393-110">This opens the Overview for your subscription.</span></span>
3. <span data-ttu-id="ef393-111">구독 **블레이드에서** 속성을 **클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="ef393-111">On the **Subscription** blade, click **Properties**.</span></span> 
4. <span data-ttu-id="ef393-112">서비스 관리 **단추를** 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="ef393-112">Click the **Service Admin** button.</span></span>
5. <span data-ttu-id="ef393-113">서비스 관리자로 설정할 사용자의 전자 메일을 입력하고 확인을 **클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="ef393-113">Enter the email of the user whom you want to set as a Service Administrator and click **OK**.</span></span>

<span data-ttu-id="ef393-114">**공동 관리자 추가/변경/제거**</span><span class="sxs-lookup"><span data-stu-id="ef393-114">**Add/Change/Remove Co-administrator**</span></span>

1. <span data-ttu-id="ef393-115">[Azure Portal에 서비스](https://ms.portal.azure.com/#home) 관리자로 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="ef393-115">Log in to the [Azure portal](https://ms.portal.azure.com/#home) as a Service Administrator.</span></span>
2. <span data-ttu-id="ef393-116">구독을 [열고](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) 구독을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="ef393-116">Open [Subscriptions](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) and select a subscription.</span></span> <span data-ttu-id="ef393-117">공동 관리자에게는 구독 범위에서만 할당할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ef393-117">(Co-adminstrators can only be assigned at the subscription scope.)</span></span>
3. <span data-ttu-id="ef393-118">**IAM(액세스 제어)** 클래식 관리자로 이동하여 공동 관리자 추가를 추가하여 공동 관리자 추가 창을 열 수 있습니다(공동 관리자 추가 옵션을 사용하지 않도록 설정하면 권한이 없다는  >  **Classic administrators**  >  **Add**  >  **Add co-administrator** 것입니다). **Add co-admin**</span><span class="sxs-lookup"><span data-stu-id="ef393-118">Navigate to **Access control (IAM)** > **Classic administrators** > **Add** > **Add co-administrator** to open the **Add co-admin** pane (If the Add co-administrator option is disabled, it denotes that you do not have permissions).</span></span>
4. <span data-ttu-id="ef393-119">추가할 사용자를 선택하고 추가를 **클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="ef393-119">Select the user whom you want to add and click **Add**.</span></span>

<span data-ttu-id="ef393-120">**더 알아보세요:**</span><span class="sxs-lookup"><span data-stu-id="ef393-120">**Learn more:**</span></span>
- [<span data-ttu-id="ef393-121">공동 관리자 추가</span><span class="sxs-lookup"><span data-stu-id="ef393-121">Add a Co-Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="ef393-122">공동 관리자 제거</span><span class="sxs-lookup"><span data-stu-id="ef393-122">Remove a co-administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="ef393-123">서비스 관리자 변경</span><span class="sxs-lookup"><span data-stu-id="ef393-123">Change the Service Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="ef393-124">계정 관리자 보기</span><span class="sxs-lookup"><span data-stu-id="ef393-124">View the Account Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="ef393-125">RBAC 및 Azure Portal을 사용하여 액세스 관리</span><span class="sxs-lookup"><span data-stu-id="ef393-125">Manage access using RBAC and Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

<span data-ttu-id="ef393-126">**Azure AD(Active Directory)를 사용하여 사용자 추가/삭제**</span><span class="sxs-lookup"><span data-stu-id="ef393-126">**Add/delete users using Azure Active Directory (AD)**</span></span>

<span data-ttu-id="ef393-127">새 사용자를 추가하거나 Azure AD(Azure Active Directory) 조직에서 기존 사용자를 삭제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ef393-127">You can add new users or delete existing users from your Azure Active Directory (Azure AD) organization:</span></span>

1. <span data-ttu-id="ef393-128">새 사용자를 추가하려면 [Azure Portal에](https://ms.portal.azure.com/#home) 조직의 사용자 관리자로 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="ef393-128">To add a new user, log in to the [Azure portal](https://ms.portal.azure.com/#home) as a User-administrator for the organization.</span></span>
2. <span data-ttu-id="ef393-129">**Azure Active Directory를 선택하고** 사용자를 선택한 다음 새 사용자를 **클릭합니다.** **Users**</span><span class="sxs-lookup"><span data-stu-id="ef393-129">Select **Azure Active Directory**, select **Users** and then click **New user**.</span></span>
3. <span data-ttu-id="ef393-130">사용자 **페이지에서** 필요한 정보를 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="ef393-130">On the **User** page, fill out the required information.</span></span> <span data-ttu-id="ef393-131">**만들기** 를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="ef393-131">Click **Create**.</span></span> <span data-ttu-id="ef393-132">사용자가 만들어지며 Azure AD 테넌트에 추가됩니다.</span><span class="sxs-lookup"><span data-stu-id="ef393-132">The user is created and added to your Azure AD tenant.</span></span>

<span data-ttu-id="ef393-133">**자세한 내용은 다음을 다국어로 추가합니다.**</span><span class="sxs-lookup"><span data-stu-id="ef393-133">**Learn more**:</span></span>

- [<span data-ttu-id="ef393-134">새 사용자 추가</span><span class="sxs-lookup"><span data-stu-id="ef393-134">Add a new user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="ef393-135">사용자 삭제</span><span class="sxs-lookup"><span data-stu-id="ef393-135">Delete a user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="ef393-136">Azure Active Directory를 사용하여 사용자의 프로필 정보 추가 또는 업데이트</span><span class="sxs-lookup"><span data-stu-id="ef393-136">Add or update a user's profile information using Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

<span data-ttu-id="ef393-137">**권장 문서**</span><span class="sxs-lookup"><span data-stu-id="ef393-137">**Recommended documents**</span></span>

- [<span data-ttu-id="ef393-138">RBAC(역할 기반 액세스 제어)란?</span><span class="sxs-lookup"><span data-stu-id="ef393-138">What is role-based access control (RBAC)?</span></span>](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [<span data-ttu-id="ef393-139">Azure의 다양한 역할 이해</span><span class="sxs-lookup"><span data-stu-id="ef393-139">Understand the different roles in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [<span data-ttu-id="ef393-140">Azure Active Directory의 관리자 역할 권한</span><span class="sxs-lookup"><span data-stu-id="ef393-140">Administrator role permissions in Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [<span data-ttu-id="ef393-141">자습서: RBAC 및 Azure Portal을 사용하여 사용자에게 액세스 권한 부여</span><span class="sxs-lookup"><span data-stu-id="ef393-141">Tutorial: Grant access for a user using RBAC and the Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [<span data-ttu-id="ef393-142">Azure에서 RBAC 문제 해결</span><span class="sxs-lookup"><span data-stu-id="ef393-142">Troubleshoot RBAC in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [<span data-ttu-id="ef393-143">Azure 관리 그룹을 사용하여 리소스 구성</span><span class="sxs-lookup"><span data-stu-id="ef393-143">Organize your resources with Azure management groups</span></span>](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [<span data-ttu-id="ef393-144">전자 메일을 통해 Azure 송장의 복사본을 요청하는 방법</span><span class="sxs-lookup"><span data-stu-id="ef393-144">How to request copy of Azure invoice via email</span></span>](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [<span data-ttu-id="ef393-145">Azure에서 신용 카드 또는 직불 카드를 추가, 업데이트 또는 제거하는 방법</span><span class="sxs-lookup"><span data-stu-id="ef393-145">How to add, update or remove a credit or debit card from Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [<span data-ttu-id="ef393-146">구독 관리(다시 활성화/취소/전환)</span><span class="sxs-lookup"><span data-stu-id="ef393-146">Manage (Reactivate/Cancel/Switch) subscription</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



