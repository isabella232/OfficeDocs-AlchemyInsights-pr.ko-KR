---
title: 송장 결제로 전환(체크/전신 송금) - 레거시 WD
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
ms.openlocfilehash: 1be90771f994e832960383b1cb5e0bee8f5b08f8
ms.sourcegitcommit: b561c339926fad609950ac92744c3cd91e0a68fa
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/21/2020
ms.locfileid: "49722824"
---
# <a name="switch-to-invoice-pay-chequewire-transfer---legacy-wd"></a><span data-ttu-id="3c6fb-102">송장 결제로 전환(체크/전신 송금) - 레거시 WD</span><span class="sxs-lookup"><span data-stu-id="3c6fb-102">Switch to invoice pay (cheque/wire transfer) - Legacy WD</span></span>

<span data-ttu-id="3c6fb-103">송장으로 결제로 전환하면 송장 날짜 30일 이내에 청구서를 결제하게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="3c6fb-103">If you switch to pay by invoice, that means you will pay your bill within 30 days of the invoice date.</span></span> <span data-ttu-id="3c6fb-104">Azure 구독 요금을 송장으로 결제할 자격이 되기 위해 Azure 지원에 요청을 제출합니다.</span><span class="sxs-lookup"><span data-stu-id="3c6fb-104">To become eligible to pay for your Azure subscription by invoice, submit a request to Azure support.</span></span> <span data-ttu-id="3c6fb-105">요청이 승인되면 Azure Portal에서 구독을 송장 결제로 [전환할 수 있습니다.](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="3c6fb-105">Once your request is approved, you can switch a subscription to invoice pay in the [Azure portal](https://portal.azure.com/).</span></span>

<span data-ttu-id="3c6fb-106">**계속하기 전에 송장 결제 옵션 요청에 대한 다음 요구 사항/제한 사항을 검토하세요.**</span><span class="sxs-lookup"><span data-stu-id="3c6fb-106">**Before you proceed further, review the following requirements/limitations on requesting invoice payment option:**</span></span>

- <span data-ttu-id="3c6fb-107">[Azure Portal에 로그인하고](https://portal.azure.com/) 결제 방법으로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="3c6fb-107">Log in to [Azure portal](https://portal.azure.com/) and navigate to payment methods.</span></span> <span data-ttu-id="3c6fb-108">송장 결제가 이미 사전 승인되어 있는지 확인</span><span class="sxs-lookup"><span data-stu-id="3c6fb-108">Check if you are already pre-approved for invoice payment.</span></span>
- <span data-ttu-id="3c6fb-109">송장 급여는 개인 계정이 아니라 비즈니스 계정에만 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3c6fb-109">Invoice pay is only available for business accounts, not for personal accounts.</span></span>
- <span data-ttu-id="3c6fb-110">송장 결제로 전환하기 전에 미지급 요금을 모두 지불해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="3c6fb-110">You must pay all outstanding charges before switching to invoice pay.</span></span>
- <span data-ttu-id="3c6fb-111">지원 팀은 계정을 검토하여 송장 결제 모드에 적합한지 여부를 확인할 것입니다.</span><span class="sxs-lookup"><span data-stu-id="3c6fb-111">The support team will review the account to determine if it is eligible for invoice mode of payment.</span></span>
- <span data-ttu-id="3c6fb-112">마켓플레이스 제3자 서비스에는 송장 결제 모드가 지원되지 않습니다. 현재 구독을 마켓플레이스 또는 제3자 서비스가 포함된 송장으로 전환하려는 경우 전환하기 전에 이러한 서비스를 삭제해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="3c6fb-112">Invoice mode of payment is not supported for marketplace 3rd party services; if you intend to switch a current subscription to an invoice that contains marketplace or 3rd party services, these services must be deleted before switching.</span></span> <span data-ttu-id="3c6fb-113">향후 마켓플레이스 서비스의 경우 먼저 신용 카드에 별도의 구독을 구입한 다음 마켓플레이스 제3자 서비스를 구매하거나 배포합니다.</span><span class="sxs-lookup"><span data-stu-id="3c6fb-113">For future marketplace services, purchase a separate subscription on credit card first and then purchase or deploy marketplace 3rd party services.</span></span>
- <span data-ttu-id="3c6fb-114">송장 결제로 전환한 후 신용 카드 또는 직불 카드 결제로 다시 전환할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="3c6fb-114">Once you switch to invoice pay, you can't switch back to credit or debit card payment.</span></span>

<span data-ttu-id="3c6fb-115">*송장으로* 결제가 승인되면 Azure Portal에서 수장 또는 전신 송금을 통해 Azure 구독을 송장 결제로 전환할  [수 있습니다.](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="3c6fb-115">*Once you're approved to pay by invoice*, you can switch your Azure subscription to the invoice pay via cheque or wire transfer in the [Azure portal](https://portal.azure.com/).</span></span>
<span data-ttu-id="3c6fb-116">이를 위해</span><span class="sxs-lookup"><span data-stu-id="3c6fb-116">To do that:</span></span>

1. <span data-ttu-id="3c6fb-117">계정 관리자로 [Azure Portal에](https://portal.azure.com/)   로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="3c6fb-117">Sign in to the [Azure portal](https://portal.azure.com/) as the Account Administrator.</span></span> <span data-ttu-id="3c6fb-118">비용 관리 **+ 청구를 검색하고 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="3c6fb-118">Search for and select **Cost Management + Billing**.</span></span>
2. <span data-ttu-id="3c6fb-119">송장 결제로 전환할 구독을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="3c6fb-119">Select the subscription you would like to switch to invoice payment.</span></span> <span data-ttu-id="3c6fb-120">결제 **방법을 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="3c6fb-120">Select **Payment methods**.</span></span>
3. <span data-ttu-id="3c6fb-121">명령 표시줄에서 송장으로 **결제 단추를** 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="3c6fb-121">In the command bar, click the **Pay by invoice** button.</span></span>

<span data-ttu-id="3c6fb-122">**권장 문서**</span><span class="sxs-lookup"><span data-stu-id="3c6fb-122">**Recommended Documents**</span></span>

- [<span data-ttu-id="3c6fb-123">Azure 청구 송장 및 사용 현황 데이터 요청/다운로드/보기</span><span class="sxs-lookup"><span data-stu-id="3c6fb-123">Request/Download/View your Azure billing invoice and usage data</span></span>](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date)
- [<span data-ttu-id="3c6fb-124">Azure 송장을 받은 편지함으로 직접 전자 메일로 전송하는 방법</span><span class="sxs-lookup"><span data-stu-id="3c6fb-124">How to email Azure invoices directly to your inbox</span></span>](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date)
- [<span data-ttu-id="3c6fb-125">송장으로 결제</span><span class="sxs-lookup"><span data-stu-id="3c6fb-125">Pay by invoice</span></span>](https://docs.microsoft.com/azure/billing/billing-how-to-pay-by-invoice)
- [<span data-ttu-id="3c6fb-126">자세한 사용 요금 이해</span><span class="sxs-lookup"><span data-stu-id="3c6fb-126">Understand detailed usage charges</span></span>](https://docs.microsoft.com/azure/billing/billing-understand-your-bill)
- [<span data-ttu-id="3c6fb-127">송장의 용어 이해</span><span class="sxs-lookup"><span data-stu-id="3c6fb-127">Understand terms on your invoice</span></span>](https://docs.microsoft.com/azure/billing/billing-understand-your-invoice)
- [<span data-ttu-id="3c6fb-128">소유권을 이전하는 방법</span><span class="sxs-lookup"><span data-stu-id="3c6fb-128">How to transfer ownership</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer)
