---
title: MCA와 관련된 판매 및 청구지 주소 업데이트 - 권장 단계
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004166"
- "7325"
ms.openlocfilehash: 8cdd2c64a95e88eb2fb4624c6e2696f77b75e198
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49652185"
---
# <a name="update-sold-to-and-bill-to-address-associated-to-your-mca---recommended-steps"></a><span data-ttu-id="25ee2-102">MCA와 관련된 판매 및 청구지 주소 업데이트 - 권장 단계</span><span class="sxs-lookup"><span data-stu-id="25ee2-102">Update sold-to and bill-to address associated to your MCA - recommended steps</span></span>

<span data-ttu-id="25ee2-103">MCA(Microsoft 고객 계약)에 연결된 판매 및 청구지 주소를 업데이트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="25ee2-103">You can update the sold-to and bill-to address associated to your Microsoft Customer Agreement (MCA).</span></span> 

> [!NOTE]
> <span data-ttu-id="25ee2-104">사용자 관리자만 Azure Active Directory 사용자 프로필 정보를 변경할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="25ee2-104">Only a user administrator can make changes to the Azure Active Directory user profile information.</span></span> <span data-ttu-id="25ee2-105">사용자 관리자 역할이 할당되지 않은 경우 사용자 관리자에게 문의하십시오.</span><span class="sxs-lookup"><span data-stu-id="25ee2-105">If you're not assigned the user administrator role, contact your user administrator.</span></span> <span data-ttu-id="25ee2-106">사용자 프로필을 변경하는 데 대한 자세한 내용은 Azure Active Directory를 사용하여 사용자의 프로필 정보 추가 또는 [업데이트를 참조하세요.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="25ee2-106">For more information about changing a user's profile, see [Add or update a user's profile information using Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal).</span></span>

<span data-ttu-id="25ee2-107">**판매 주소** - 판매된 주소는 조직 또는 개인의 주소 및 연락처 정보로, 청구 계좌를 담당합니다.</span><span class="sxs-lookup"><span data-stu-id="25ee2-107">**Sold-to address** - The sold-to address is the address and the contact information of the organization or the individual, who is responsible for a billing account.</span></span> <span data-ttu-id="25ee2-108">청구 계정에 대해 생성된 모든 송장에 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="25ee2-108">It's displayed in all the invoices generated for the billing account.</span></span>

<span data-ttu-id="25ee2-109">**청구지 주소** - 청구지 주소는 청구 계정에 대해 생성된 송장을 담당하는 조직 또는 개인의 주소 및 연락처 정보입니다.</span><span class="sxs-lookup"><span data-stu-id="25ee2-109">**Bill-to address** - The bill-to address is the address and the contact information of the organization or the individual, who is responsible for the invoices generated for a billing account.</span></span> <span data-ttu-id="25ee2-110">MCA에 대한 청구 계정의 경우 각 청구 프로필에 대한 청구지 주소가 있으며 청구 프로필에 대해 생성된 송장에 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="25ee2-110">For a billing account for an MCA, there's a bill-to address for each billing profile and it's displayed in the invoice generated for the billing profile.</span></span>

<span data-ttu-id="25ee2-111">**판매된 MCA** 청구 계정을 업데이트하려면:</span><span class="sxs-lookup"><span data-stu-id="25ee2-111">**To update an MCA billing account sold-to address**:</span></span>

1. <span data-ttu-id="25ee2-112">MCA에 대한 청구 계정에 소유자 또는 참가자 역할이 있는 전자 메일 주소를 사용하여 Azure Portal에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="25ee2-112">Sign in to the Azure portal using the email address, which has an owner or a contributor role on the billing account for an MCA.</span></span>
1. <span data-ttu-id="25ee2-113">비용 관리  +  **청구를 검색합니다.**</span><span class="sxs-lookup"><span data-stu-id="25ee2-113">Search for **Cost Management** + **Billing**.</span></span>
1. <span data-ttu-id="25ee2-114">  >  **매도된 속성 업데이트를 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="25ee2-114">Click **Properties** > **Update sold-to**.</span></span>
1. <span data-ttu-id="25ee2-115">새 주소를 입력하고 저장을 **클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="25ee2-115">Enter the new address and click **Save**.</span></span>

<span data-ttu-id="25ee2-116">일부 계정은 판매된 주소가 업데이트되기 전에 추가 확인이 요구됩니다.</span><span class="sxs-lookup"><span data-stu-id="25ee2-116">Some accounts require additional verification before their sold-to address can be updated.</span></span> <span data-ttu-id="25ee2-117">계정에 수동 승인이 필요한 경우 Azure 지원에 문의해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="25ee2-117">If your account requires manual approval, you'll be asked to contact Azure support.</span></span>

<span data-ttu-id="25ee2-118">**MCA 청구 계정 주소를 업데이트하려면**</span><span class="sxs-lookup"><span data-stu-id="25ee2-118">**To update an MCA billing account address**:</span></span> 

1. <span data-ttu-id="25ee2-119">청구 계정 또는 MCA에 대한 청구 프로필에 소유자 또는 참가자 역할이 있는 전자 메일 주소를 사용하여 Azure Portal에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="25ee2-119">Sign in to the Azure portal using the email address, which has an owner or a contributor role on a billing account or a billing profile for an MCA.</span></span>
1. <span data-ttu-id="25ee2-120">비용 관리  +  **청구를 검색합니다.**</span><span class="sxs-lookup"><span data-stu-id="25ee2-120">Search for **Cost Management** + **Billing**.</span></span>
1. <span data-ttu-id="25ee2-121">청구 **프로필을 클릭하고** 청구 프로필을 선택하여 청구 주소를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="25ee2-121">Click **Billing profiles** and select a select a billing profile to update the billing address.</span></span>
1. <span data-ttu-id="25ee2-122">속성 **업데이트**  >  **주소를 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="25ee2-122">Click **Properties** > **Update address**.</span></span>
1. <span data-ttu-id="25ee2-123">새 주소를 입력하고 저장을 **클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="25ee2-123">Enter the new address and then click **Save**.</span></span>

<span data-ttu-id="25ee2-124">**권장 문서**</span><span class="sxs-lookup"><span data-stu-id="25ee2-124">**Recommended documents**</span></span>

<span data-ttu-id="25ee2-125">[Azure 청구 계정에 대한 연락처 정보 변경](https://docs.microsoft.com/azure/cost-management-billing/manage/change-azure-account-profile) </span><span class="sxs-lookup"><span data-stu-id="25ee2-125">[Change contact information for an Azure billing account](https://docs.microsoft.com/azure/cost-management-billing/manage/change-azure-account-profile) </span></span>  
[<span data-ttu-id="25ee2-126">청구 계정 설정 업데이트</span><span class="sxs-lookup"><span data-stu-id="25ee2-126">Update billing account settings</span></span>](https://docs.microsoft.com/microsoft-store/update-microsoft-store-for-business-account-settings)  
[<span data-ttu-id="25ee2-127">Azure의 Microsoft 고객 계약 관리 역할 이해</span><span class="sxs-lookup"><span data-stu-id="25ee2-127">Understand Microsoft Customer Agreement administrative roles in Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)