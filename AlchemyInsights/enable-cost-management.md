---
title: 비용 관리 사용
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599082"
---
# <a name="enable-cost-management"></a><span data-ttu-id="21ae7-102">비용 관리 사용</span><span class="sxs-lookup"><span data-stu-id="21ae7-102">Enable cost management</span></span>

<span data-ttu-id="21ae7-103">**'조직에 대해 비용이 사용하지 않도록 설정되어 있습니다.'는 무엇을 의미하나요?**</span><span class="sxs-lookup"><span data-stu-id="21ae7-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="21ae7-104">EA(기업계약) 또는 MCA(Microsoft 고객 계약) 계정을 사용하는 조직은 비용 정보 및 가격 정보에 대한 액세스를 사용하지 않도록 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="21ae7-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="21ae7-105">Azure Portal에 로그인한 후 청구 API를 사용하여 프로그래밍식으로 송장(옵트인) 및 사용 세부 정보를 받을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="21ae7-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="21ae7-106">**추가 사용자가 송장에 액세스하도록 허용하는 방법**</span><span class="sxs-lookup"><span data-stu-id="21ae7-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="21ae7-107">Azure **Portal에서 구독** 블레이드로 이동하세요.</span><span class="sxs-lookup"><span data-stu-id="21ae7-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="21ae7-108">Select **Invoices** and then **Access to invoices.**</span><span class="sxs-lookup"><span data-stu-id="21ae7-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="21ae7-109">구독 범위 역할의 사용자가 송장을 다운로드할 수 있도록 액세스를 켜고 변경 내용을 저장합니다.</span><span class="sxs-lookup"><span data-stu-id="21ae7-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="21ae7-110">계정 관리자는 전자 메일을 통해 송장을 보내도록 구성할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="21ae7-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="21ae7-111">To learn more, see [Get your invoice in email.](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?)</span><span class="sxs-lookup"><span data-stu-id="21ae7-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span></span>

<span data-ttu-id="21ae7-112">**청구 독자 역할에 사용자를 추가하는 방법**</span><span class="sxs-lookup"><span data-stu-id="21ae7-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="21ae7-113">Azure **Portal에서 구독 블레이드로** 이동하세요.</span><span class="sxs-lookup"><span data-stu-id="21ae7-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="21ae7-114">**IAM(액세스 제어)을** 선택하고 추가를 **클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="21ae7-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="21ae7-115">역할 **선택 페이지에서** 청구 **독자를** 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="21ae7-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="21ae7-116">초대할 사용자의 전자 메일을 입력한 다음 **확인을** 클릭하여 초대를 보낼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="21ae7-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="21ae7-117">초대 전자 메일에 제공된 지침에 따라 청구 독자로 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="21ae7-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="21ae7-118">자세한 내용은 청구에 대한 액세스 권한 [부여를 참조하세요.](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in)</span><span class="sxs-lookup"><span data-stu-id="21ae7-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="21ae7-119">**권장 문서**</span><span class="sxs-lookup"><span data-stu-id="21ae7-119">**Recommended documents**</span></span>

- [<span data-ttu-id="21ae7-120">EA 포털을 통해 DA 및 AO 보기 사용</span><span class="sxs-lookup"><span data-stu-id="21ae7-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="21ae7-121">비용 관리에 포함된 비용</span><span class="sxs-lookup"><span data-stu-id="21ae7-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="21ae7-122">지원되는 Microsoft Azure 제품</span><span class="sxs-lookup"><span data-stu-id="21ae7-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="21ae7-123">비용 분석의 비용 검토</span><span class="sxs-lookup"><span data-stu-id="21ae7-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="21ae7-124">청구 정보에 대한 액세스 제공</span><span class="sxs-lookup"><span data-stu-id="21ae7-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="21ae7-125">Microsoft 고객 계약에 대한 액세스 확인</span><span class="sxs-lookup"><span data-stu-id="21ae7-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






