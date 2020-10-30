---
title: 지원되는 구독 유형
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6675"
ms.openlocfilehash: 46bc60435c3f8477e9f274d90c39d0f1c6a523c6
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/28/2020
ms.locfileid: "48791477"
---
# <a name="supported-subscription-types"></a><span data-ttu-id="029ba-102">지원되는 구독 유형</span><span class="sxs-lookup"><span data-stu-id="029ba-102">Supported subscription types</span></span>

<span data-ttu-id="029ba-103">지원되는 구독 유형을 검토하여 계속 진행하세요.</span><span class="sxs-lookup"><span data-stu-id="029ba-103">Please review the supported subscription types to proceed further.</span></span>

[<span data-ttu-id="029ba-104">지원되는 구독 유형</span><span class="sxs-lookup"><span data-stu-id="029ba-104">Supported subscription types</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

<span data-ttu-id="029ba-105">**대금 청구 소유권 이전**</span><span class="sxs-lookup"><span data-stu-id="029ba-105">**Transfer billing ownership**</span></span>

<span data-ttu-id="029ba-106">이전하려는 구독이 있는 청구 계정의 [계정 관리자](https://ms.portal.azure.com/)로서 Azure Portal</span><span class="sxs-lookup"><span data-stu-id="029ba-106">Azure portal as the [Account Admin](https://ms.portal.azure.com/) of the billing account that has the subscription you want to transfer</span></span>

- <span data-ttu-id="029ba-107">**비용 관리 + 청구** 검색</span><span class="sxs-lookup"><span data-stu-id="029ba-107">Search on **Cost Management + Billing** .</span></span> <span data-ttu-id="029ba-108">왼쪽 창에서 **구독** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="029ba-108">Select **Subscriptions** from left-pane.</span></span> <span data-ttu-id="029ba-109">액세스 권한에 따라 청구 범위를 선택한 후, **구독** 혹은 **Azure 구독** 을 선택해야할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="029ba-109">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions** .</span></span>
- <span data-ttu-id="029ba-110">이전할 구독의 청구 소유권 이전을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="029ba-110">Select Transfer billing ownership for the subscription you want to transfer</span></span>
- <span data-ttu-id="029ba-111">구독에 대한 새 소유자가 될 계정의 청구 관리자인 사용자의 전자 메일 주소를 입력한 다음 **이전 요청 보내기** 를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="029ba-111">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="029ba-112">사용자는 이전 요청을 검토하는 지침이 포함된 전자 메일을 받습니다.</span><span class="sxs-lookup"><span data-stu-id="029ba-112">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="029ba-113">이전 요청을 승인하려면 사용자는 전자 메일에서 링크를 선택하고 지침을 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="029ba-113">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="029ba-114">참고: 구독의 대금 청구 소유권을 다른 Azure AD 테넌트에 있는 사용자의 계정에 이전하는 경우, 구독에서 리소스를 관리하기 위한 모든 [RBAC(역할 기반 액세스 제어)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) 할당이 영구적으로 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="029ba-114">Note: If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="029ba-115">새 소유자만 구독에서 리소스를 관리하는 데 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="029ba-115">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="029ba-116">자세한 내용은 [다른 Azure AD 테넌트에 있는 사용자에게 구독 이전](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="029ba-116">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="029ba-117">**구독의 소유권 이전**</span><span class="sxs-lookup"><span data-stu-id="029ba-117">**Transfer Ownership of Subscription**</span></span>

<span data-ttu-id="029ba-118">구독 소유권 이전 시 필수 구성 요소인 구독에서 리소스를 관리하기 위한 RBAC(역할 기반 액세스 제어)에 대한 액세스 권한을 잃게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="029ba-118">Subscription Ownership Transfer prerequisites role based access (RBAC) to manage resources in the subscription lose their access.</span></span> <span data-ttu-id="029ba-119">기존 구독을 테넌트에 추가하는 방법에 대한 자세한 내용은 [Azure 구독을 Azure Active Directory에 연결 또는 추가](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="029ba-119">For more information about adding an existing subscription to a tenant, see [Associate or add an Azure subscription to Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

- <span data-ttu-id="029ba-120">현재 대금 청구 주기에 기존 미납 금액이 있는 구독을 이전하면 새 계정의 새 결제 방법으로 이전되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="029ba-120">Subscription Transfer with an existing outstanding amount from the current billing cycle will not be transferred to the new payment instrument in the new account.</span></span> <span data-ttu-id="029ba-121">새 계정에서 사용자가 사용할 수 있는 유일한 정보는 구독에 대 한 마지막 월간 비용입니다.</span><span class="sxs-lookup"><span data-stu-id="029ba-121">The only information available to the users in new account is the last month's cost for your subscription.</span></span> <span data-ttu-id="029ba-122">나머지 사용 및 청구 기록은 구독과 함께 전송 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="029ba-122">The rest of the usage and billing history does not transfer with the subscription.</span></span>
- <span data-ttu-id="029ba-123">엔터프라이즈 규약 (EA) 구독의 대금 청구 소유권 전송은 현재 엔터프라이즈 규약 포털 에서만 지원 됩니다.</span><span class="sxs-lookup"><span data-stu-id="029ba-123">Transfer billing ownership of Enterprise Agreement (EA) subscriptions is currently supported in the Enterprise Agreement Portal only</span></span>
- <span data-ttu-id="029ba-124">Visual Studio, BizSpark, Microsoft 파트너 네트워크와 같은 신용을 바탕으로 한 구독을 새 사용자에게 이전하려면 Visual Studio/Microsoft 파트너 네트워크 라이선스가 있어야 이전 요청을 수락할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="029ba-124">Transferring a credit-oriented subscription like Visual Studio, BizSpark, Microsoft Partner Network to a new user requires to have a Visual Studio/Microsoft partner network license to accept the transfer request</span></span>
- <span data-ttu-id="029ba-125">가상 컴퓨터, 디스크 및 웹 사이트와 같은 모든 리소스는 새 계정으로 이전됩니다.</span><span class="sxs-lookup"><span data-stu-id="029ba-125">All resources like Virtual Machines, disks, and websites transfer to the new account successfully.</span></span> <span data-ttu-id="029ba-126">다음 리소스는 테넌트 간의 구독 이전 시 영향을 받을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="029ba-126">The following resources could be affected in a cross-tenant subscription transfer:</span></span>

<span data-ttu-id="029ba-127">**Azure AD 도메인 서비스**</span><span class="sxs-lookup"><span data-stu-id="029ba-127">**Azure AD Domain Services**</span></span>

<span data-ttu-id="029ba-128">Azure Key Vault</span><span class="sxs-lookup"><span data-stu-id="029ba-128">Azure Key Vaults</span></span>

- <span data-ttu-id="029ba-129">특히 고객이 Azure Active Directory 관련 인증을 사용하는 경우, [SQL 관련 사용자 및 데이터베이스](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support)가 영향을 받을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="029ba-129">[SQL related users and databases](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) could be impacted, especially if the customer uses an Azure Active Directory related authentication</span></span>
- <span data-ttu-id="029ba-130">Azure Active Directory 인증을 사용하여 구성된 **App Services** 가 영향을 받을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="029ba-130">**App Services** configured with Azure Active Directory authentication could be impacted</span></span>
- <span data-ttu-id="029ba-131">Azure 구독에 연결된 **Visual Studio Team** Services 계정은 연결된 Azure 구독이 취소될 때 일시적으로 액세스 권한을 잃을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="029ba-131">**Visual Studio Team** Services accounts connected to Azure subscriptions may temporarily lose access when the connected Azure subscription is cancelled</span></span>

<span data-ttu-id="029ba-132">**추천 문서**</span><span class="sxs-lookup"><span data-stu-id="029ba-132">**Recommended Documents**</span></span>

<span data-ttu-id="029ba-133">대금 청구 소유권을 수락한 후의 단계:</span><span class="sxs-lookup"><span data-stu-id="029ba-133">Steps after accepting billing ownership:</span></span>

- <span data-ttu-id="029ba-134">대금 청구 소유권을 유지하되 구독의 유형을 변경하려면 [Azure 구독을 다른 플랜으로 전환](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="029ba-134">To retain billing ownership, but change the type of your subscription, refer: [Switch your Azure subscription to another offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>
- [<span data-ttu-id="029ba-135">Visual Studio, Microsoft 파트너 네트워크 (MPN) 및 종량제 개발/테스트 구독의 이전</span><span class="sxs-lookup"><span data-stu-id="029ba-135">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="029ba-136">EA(엔터프라이즈 계약) 구독의 대금 청구 소유권 이전</span><span class="sxs-lookup"><span data-stu-id="029ba-136">Transfer billing ownership of Enterprise Agreement (EA) subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [<span data-ttu-id="029ba-137">소유권 이전 FAQ</span><span class="sxs-lookup"><span data-stu-id="029ba-137">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="029ba-138">소유권 이전 문제 해결</span><span class="sxs-lookup"><span data-stu-id="029ba-138">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)