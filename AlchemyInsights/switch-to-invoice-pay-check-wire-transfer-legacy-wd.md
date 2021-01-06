---
title: 송장으로 결제로 전환(체크/전신 송금)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004168"
- "7343"
ms.openlocfilehash: c4c78d634cdef711423f573439c5091befedef34
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755409"
---
# <a name="switch-to-pay-by-invoice-chequewire-transfer"></a><span data-ttu-id="69b6c-102">송장으로 결제로 전환(체크/전신 송금)</span><span class="sxs-lookup"><span data-stu-id="69b6c-102">Switch to pay by invoice (cheque/wire transfer)</span></span>

<span data-ttu-id="69b6c-103">문제 설명에 따라 해결 방법을 찾은 것입니다.</span><span class="sxs-lookup"><span data-stu-id="69b6c-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="69b6c-104">대부분의 고객은 설명서를 따라 문제를 직접 해결할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="69b6c-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="69b6c-105">송장으로 결제로 전환하면 송장 날짜 30일 이내에 청구서를 결제하게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="69b6c-105">If you switch to pay by invoice, that means you will pay your bill within 30 days of the invoice date.</span></span> <span data-ttu-id="69b6c-106">송장으로 Azure 구독 비용을 지불할 자격이 되기 위해 Azure 지원에 요청을 제출합니다.</span><span class="sxs-lookup"><span data-stu-id="69b6c-106">To become eligible to pay for your Azure subscription by invoice, submit a request to Azure support.</span></span> <span data-ttu-id="69b6c-107">요청이 승인되면 Azure Portal에서 구독을 송장 결제로 [전환할 수 있습니다.](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="69b6c-107">Once your request is approved, you can switch a subscription to invoice pay in the [Azure portal](https://portal.azure.com/).</span></span>

<span data-ttu-id="69b6c-108">**계속하기 전에 송장 결제 옵션 요청에 대한 다음 요구 사항/제한 사항을 검토하세요.**</span><span class="sxs-lookup"><span data-stu-id="69b6c-108">**Before you proceed further, review the following requirements/limitations on requesting invoice payment option:**</span></span>

- <span data-ttu-id="69b6c-109">[Azure Portal에 로그인하고](https://portal.azure.com/) 결제 방법을 탐색합니다.</span><span class="sxs-lookup"><span data-stu-id="69b6c-109">Log in to [Azure portal](https://portal.azure.com/) and navigate to payment methods.</span></span> <span data-ttu-id="69b6c-110">송장 결제가 이미 사전 승인되어 있는지 확인</span><span class="sxs-lookup"><span data-stu-id="69b6c-110">Check if you are already pre-approved for invoice payment.</span></span>
- <span data-ttu-id="69b6c-111">송장 급여는 개인 계정이 아니라 비즈니스 계정에만 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="69b6c-111">Invoice pay is only available for business accounts, not for personal accounts.</span></span>
- <span data-ttu-id="69b6c-112">송장 결제로 전환하기 전에 미지급 요금을 모두 지불해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="69b6c-112">You must pay all outstanding charges before switching to invoice pay.</span></span>
- <span data-ttu-id="69b6c-113">지원 팀은 계정을 검토하여 송장 결제 모드가 적합한지 여부를 판단합니다.</span><span class="sxs-lookup"><span data-stu-id="69b6c-113">The support team will review the account to determine if it is eligible for invoice mode of payment.</span></span>
- <span data-ttu-id="69b6c-114">마켓플레이스 제3자 서비스에는 송장 결제 모드가 지원되지 않습니다. 현재 구독을 마켓플레이스 또는 제3자 서비스가 포함된 송장으로 전환하려는 경우 전환하기 전에 이러한 서비스를 삭제해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="69b6c-114">Invoice mode of payment is not supported for marketplace 3rd party services; if you intend to switch a current subscription to an invoice that contains marketplace or 3rd party services, these services must be deleted before switching.</span></span> <span data-ttu-id="69b6c-115">향후 마켓플레이스 서비스의 경우 먼저 신용 카드에 별도의 구독을 구입한 다음 마켓플레이스 제3자 서비스를 구매하거나 배포합니다.</span><span class="sxs-lookup"><span data-stu-id="69b6c-115">For future marketplace services, purchase a separate subscription on credit card first and then purchase or deploy marketplace 3rd party services.</span></span>
- <span data-ttu-id="69b6c-116">송장 결제로 전환한 후 신용 카드 또는 직불 카드 결제로 다시 전환할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="69b6c-116">Once you switch to invoice pay, you can't switch back to credit or debit card payment.</span></span>

<span data-ttu-id="69b6c-117">*송장으로* 결제가 승인되면 Azure Portal에서 수장 또는 전신 송금을 통해 Azure 구독을 송장 결제로 전환할  [수 있습니다.](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="69b6c-117">*Once you're approved to pay by invoice*, you can switch your Azure subscription to the invoice pay via cheque or wire transfer in the [Azure portal](https://portal.azure.com/).</span></span>
<span data-ttu-id="69b6c-118">이를 위해</span><span class="sxs-lookup"><span data-stu-id="69b6c-118">To do that:</span></span>

1. <span data-ttu-id="69b6c-119">계정 관리자로 [Azure Portal에](https://portal.azure.com/)   로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="69b6c-119">Sign in to the [Azure portal](https://portal.azure.com/) as the Account Administrator.</span></span> <span data-ttu-id="69b6c-120">비용 관리 **+ 청구를 검색하고 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="69b6c-120">Search for and select **Cost Management + Billing**.</span></span>
2. <span data-ttu-id="69b6c-121">송장 결제로 전환할 구독을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="69b6c-121">Select the subscription you would like to switch to invoice payment.</span></span> <span data-ttu-id="69b6c-122">결제 **방법을 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="69b6c-122">Select **Payment methods**.</span></span>
3. <span data-ttu-id="69b6c-123">명령 표시줄에서 송장으로 **결제 단추를** 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="69b6c-123">In the command bar, click the **Pay by invoice** button.</span></span>

<span data-ttu-id="69b6c-124">**추천 문서**</span><span class="sxs-lookup"><span data-stu-id="69b6c-124">**Recommended Documents**</span></span>

- [<span data-ttu-id="69b6c-125">Azure 청구 송장 및 사용 현황 데이터 요청/다운로드/보기</span><span class="sxs-lookup"><span data-stu-id="69b6c-125">Request/Download/View your Azure billing invoice and usage data</span></span>](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date)
- [<span data-ttu-id="69b6c-126">Azure 송장을 받은 편지함으로 직접 전자 메일로 전송하는 방법</span><span class="sxs-lookup"><span data-stu-id="69b6c-126">How to email Azure invoices directly to your inbox</span></span>](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date)
- [<span data-ttu-id="69b6c-127">송장으로 결제</span><span class="sxs-lookup"><span data-stu-id="69b6c-127">Pay by invoice</span></span>](https://docs.microsoft.com/azure/billing/billing-how-to-pay-by-invoice)
- [<span data-ttu-id="69b6c-128">자세한 사용 요금 이해</span><span class="sxs-lookup"><span data-stu-id="69b6c-128">Understand detailed usage charges</span></span>](https://docs.microsoft.com/azure/billing/billing-understand-your-bill)
- [<span data-ttu-id="69b6c-129">송장의 용어 이해</span><span class="sxs-lookup"><span data-stu-id="69b6c-129">Understand terms on your invoice</span></span>](https://docs.microsoft.com/azure/billing/billing-understand-your-invoice)
- [<span data-ttu-id="69b6c-130">소유권을 이전하는 방법</span><span class="sxs-lookup"><span data-stu-id="69b6c-130">How to transfer ownership</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer)
