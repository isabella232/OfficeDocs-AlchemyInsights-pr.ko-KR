---
title: 예약된 인스턴스 구입에 대한 청구
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 6cdcb5af27a475cc838eb434ff025eb18356360c
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/30/2020
ms.locfileid: "48816034"
---
# <a name="billing-for-reserved-instance-purchase"></a><span data-ttu-id="00fb9-102">예약된 인스턴스 구입에 대한 청구</span><span class="sxs-lookup"><span data-stu-id="00fb9-102">Billing for Reserved Instance purchase</span></span>

<span data-ttu-id="00fb9-103">예약된 인스턴스 구입은 구입 시 선택하는 구독과 연결된 결제 방법으로 요금이 청구됩니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-103">The reserved instance purchase is charged to the payment method tied to the subscription that you select at the time of purchase.</span></span> <span data-ttu-id="00fb9-104">구독 유형은 엔터프라이즈 계약(제품 번호: MS-AZR-0017P), 종량제(제품 번호: MS-AZR-0003P), Microsoft 고객 계약이나 CSP여야 합니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-104">The subscription type must be an enterprise agreement (offer number: MS-AZR-0017P), Pay-As-You-Go (offer number: MS-AZR-0003P), Microsoft Customer Agreement or CSP.</span></span>

- <span data-ttu-id="00fb9-105">엔터프라이즈 구독의 경우, 요금은 등록자의 금액 약정 잔액에서 공제되거나 초과 사용 기간으로 부과됩니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-105">For an enterprise subscription, the charges are deducted from the enrollment's monetary commitment balance or charged as overage</span></span>
- <span data-ttu-id="00fb9-106">종량제 구독의 경우 구독에 대한 신용 카드 또는 청구서 지불 방법으로 요금이 청구됩니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-106">For Pay-As-You-Go subscription, the charges are billed to the credit card or invoice payment method on the subscription</span></span>

<span data-ttu-id="00fb9-107">**예약 취소**</span><span class="sxs-lookup"><span data-stu-id="00fb9-107">**Cancelling Reservation**</span></span>

- <span data-ttu-id="00fb9-108">**셀프 서비스:**[Azure 포털](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)을 사용하여 직접 예약된 인스턴스를 취소하거나 교환할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-108">**Self-service:** You can cancel or exchange a reserved instance yourself using [Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade).</span></span> <span data-ttu-id="00fb9-109">예약을 선택하고 환불 또는 교환을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-109">Select the reservation and click on refund or exchange.</span></span> <span data-ttu-id="00fb9-110">교환 또는 환불을 하려면 예약 순서에 대한 소유자 액세스 권한이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-110">Note that you must have owner access on the Reservation Order to exchange or refund.</span></span> <span data-ttu-id="00fb9-111">예약으로만 액세스하는 경우에는 환불이나 교환 처리를 진행할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-111">Access to only the Reservation will not let you proceed with refund or exchange.</span></span> <span data-ttu-id="00fb9-112">예약 순서 소유자에게 예약 순서에 대한 소유자 액세스 권한을 요청합니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-112">Ask the Reservation Order owner to give you owner access to the Reservation Order</span></span>
- <span data-ttu-id="00fb9-113">**교환 정책:** 동일한 유형의 다른 예약으로 교환할 수 있습니다. 예약 변경에 대한 **벌금은 없습니다** .</span><span class="sxs-lookup"><span data-stu-id="00fb9-113">**Exchange policy:** You can exchange a reservation for another reservation of the same type – there are **no penalties** on reservation exchange.</span></span> <span data-ttu-id="00fb9-114">새 예약을 사용하는 총 약정 금액은 교환되는 예약의 환불 금액과 차후의 월간 지불액(해당하는 경우)의 합계를 초과해야 합니다. </span><span class="sxs-lookup"><span data-stu-id="00fb9-114">The total commitment with new reservation should be greater than the sum of exchanged reservation’s refund amount and the future monthly payments (if applicable)</span></span>
- <span data-ttu-id="00fb9-115">**환불 정책:** 환불 금액의 합계와 취소된 차후의 지불액은 12개월의 상환 기간에 $50,000을 초과할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-115">**Refund policy:** Sum of refund and the cancelled future payments cannot exceed $50,000 USD in a 12-month rolling window.</span></span> <span data-ttu-id="00fb9-116">**현재는 환불에 대한 벌금이 없지만** 차후에는 청구할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-116">We are **currently not charging any penalty** on refunds but could charge it on future refunds</span></span>

<span data-ttu-id="00fb9-117">**예외 사항:** 셀프 서비스 교환 및 취소 기능은 미국 정부 기업 계약 고객에게는 제공되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-117">**Exceptions:** Self-service exchange and cancel capability isn't available for US Government Enterprise Agreement customers</span></span>

- <span data-ttu-id="00fb9-118">**API / PS / CLI** 지원은 취소 및 환불에 대해서는 제공되지 않음 [Azure 예약에 대한 셀프 서비스 교환 및 환불](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="00fb9-118">**API / PS / CLI** support is not available for cancellation and refunds [Self-service exchanges and refunds for Azure Reservations](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>
- <span data-ttu-id="00fb9-119">셀프 서비스 교환 및 취소 기능은 미국 정부 기업 계약 고객에게는 제공되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-119">Self-service exchange and cancel capability isn't available for US Government Enterprise Agreement customers.</span></span> <span data-ttu-id="00fb9-120">용량제를 포함하고 CSP가 지원되는 기타 미국 정부 기관용 구독 유형</span><span class="sxs-lookup"><span data-stu-id="00fb9-120">Other US Government subscription types including Pay-As-You-Go and CSP are supported</span></span>

<span data-ttu-id="00fb9-121">자세한 내용은 [return and exchange 트랜잭션이 처리 되는 방법을](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) 참조 하세요: [exchange 및 환불 정책](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) 기타 질문: [예약 된 인스턴스 문서 방문](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="00fb9-121">Learn more : [How return and exchange transactions are processed](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) Learn more : [Exchange and Refund policies](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) Other questions: [Visit reserved instance docs](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="00fb9-122">**기존에 예약된 인스턴스 교환(셀프 서비스)**</span><span class="sxs-lookup"><span data-stu-id="00fb9-122">**Exchange an existing reserved instance (Self-service)**</span></span>

<span data-ttu-id="00fb9-123">동일한 유형의 다른 예약으로 예약을 교환할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-123">You can exchange a reservation for another reservation of the same type.</span></span> <span data-ttu-id="00fb9-124">더 이상 필요하지 않은 경우 연간 최대 $50,000 USD까지의 예약을 환불할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-124">You can also refund a reservation, up to $50,000 USD per year, if you no longer need it.</span></span> <span data-ttu-id="00fb9-125">셀프 서비스 교환 및 취소 기능은 미국 정부 기업 계약 고객에게는 제공되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-125">Self-service exchange and cancel capability isn't available for US Government Enterprise Agreement customers.</span></span> <span data-ttu-id="00fb9-126">용량제를 포함하고 CSP가 지원되는 기타 미국 정부 기관용 구독 유형입니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-126">Other US Government subscription types including Pay-As-You-Go and CSP are supported.</span></span> <span data-ttu-id="00fb9-127">기존 예약을 교환하거나 환불하려면 예약 순서에 대한 소유자 액세스 권한이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-127">You must have owner access on the Reservation Order to exchange or refund an existing reservation.</span></span>

<span data-ttu-id="00fb9-128">다음 단계는 거래를 완료하기 위한 절차를 안내합니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-128">The following steps will guide on the procedure to complete the transaction</span></span>

<span data-ttu-id="00fb9-129">1. [Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-129">1.Log in to your [Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade).</span></span> <span data-ttu-id="00fb9-130">환불 하려는 예약을 선택 하 고 **Exchange** 2를 클릭 합니다. 구입 하려는 VM 제품을 선택 하 고 수량을 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-130">Select the reservations that you want to refund and click **Exchange** 2.Select the VM product that you want to purchase and type a quantity.</span></span> <span data-ttu-id="00fb9-131">[구입 하기 전에](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)새 구매 합계가 반품 합계 보다 크거나 같은지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-131">Make sure that the new purchase total is more than the return total [Determine the right size before you purchase](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).</span></span>
<span data-ttu-id="00fb9-132">3. 트랜잭션 검토 및 완료</span><span class="sxs-lookup"><span data-stu-id="00fb9-132">3.Review and complete the transaction</span></span>

<span data-ttu-id="00fb9-133">**예약된 인스턴스에 대한 환불**</span><span class="sxs-lookup"><span data-stu-id="00fb9-133">**Refund for a reserved instance**</span></span>

<span data-ttu-id="00fb9-134">예약을 환불하려면 **예약 세부 정보** 로 이동하여 **환불** 을 클릭</span><span class="sxs-lookup"><span data-stu-id="00fb9-134">To refund a reservation, go to **Reservation Details** and click **Refund**</span></span>

<span data-ttu-id="00fb9-135">**비례 배분 환불:**</span><span class="sxs-lookup"><span data-stu-id="00fb9-135">**Pro-rated refund:**</span></span>

<span data-ttu-id="00fb9-136">**환불 및 교환에 대 한 ration 및 최소 요구 사항 예** 선행 예약 예:</span><span class="sxs-lookup"><span data-stu-id="00fb9-136">**Pro-ration and minimum requirement examples for refund and exchange** Upfront reservation example:</span></span>

- <span data-ttu-id="00fb9-137">1월 1일에 1년의 기간을 $120에 구매</span><span class="sxs-lookup"><span data-stu-id="00fb9-137">You purchase a one-year term RI for $120 on January 1</span></span>
- <span data-ttu-id="00fb9-138">4월 7일에 이 예약을 환불 혹은 교환하고자 함</span><span class="sxs-lookup"><span data-stu-id="00fb9-138">On April 7th you want to refund or exchange this reservation</span></span>
- <span data-ttu-id="00fb9-139">이 예약은 97일간에 제공되었기 때문에 (1-97/365) \* $120을 환불 받습니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-139">Since the reservation has been live for 97 days, you will get (1-97/365) \* $120 back.</span></span> <span data-ttu-id="00fb9-140">(즉, $88.1).</span><span class="sxs-lookup"><span data-stu-id="00fb9-140">(i.e. $88.1).</span></span> <span data-ttu-id="00fb9-141">현재 환불에 대한 벌금은 없습니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-141">There is currently no penalty on refunds</span></span>
- <span data-ttu-id="00fb9-142">교환할 경우, 새 구매는 $88.1을 초과해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-142">If exchanging, your new purchase should be greater than $88.1</span></span>
- <span data-ttu-id="00fb9-143">현재 환불에 대한 벌금은 없습니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-143">There is no penalty on refunds currently</span></span>

<span data-ttu-id="00fb9-144">**청구 계획 예약 예시:**</span><span class="sxs-lookup"><span data-stu-id="00fb9-144">**Billing plan reservation example:**</span></span>

- <span data-ttu-id="00fb9-145">1년 기간의 RI를 월간 $10에 구매</span><span class="sxs-lookup"><span data-stu-id="00fb9-145">You purchase a one-year term RI for $10 per month</span></span>
- <span data-ttu-id="00fb9-146">4월 7일에 이 예약을 환불 혹은 교환하고자 함</span><span class="sxs-lookup"><span data-stu-id="00fb9-146">On April 7th you want to refund or exchange this reservation</span></span>
- <span data-ttu-id="00fb9-147">마지막 결재가 7일 전에 처리되었으므로 (1-7/31) \* $10을 환불 받습니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-147">Since the last payment happened 7 days, you will get (1-7/31) \* $10 back.</span></span> <span data-ttu-id="00fb9-148">(즉, $7.74)</span><span class="sxs-lookup"><span data-stu-id="00fb9-148">(i.e. $7.74)</span></span>
- <span data-ttu-id="00fb9-149">이후의 결제는 $80입니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-149">The future payments cancelled are $ 80.</span></span> <span data-ttu-id="00fb9-150">현재 환불에 대한 벌금은 없습니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-150">There is currently no penalty on refunds</span></span>
- <span data-ttu-id="00fb9-151">이 취소는 귀하의 환불 한도 $50,000에서 $87.74를 차감합니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-151">This cancellation will deduct $87.74 from you’re the $50,000 refund limit</span></span>
- <span data-ttu-id="00fb9-152">교환할 경우, 신규 구매의 총액은 $87.74을 초과해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-152">If exchanging, the total value of new purchase should be greater than $87.74</span></span>

<span data-ttu-id="00fb9-153">**마지막 대금 청구 기간에 대 한 송장을 볼 수 없음**</span><span class="sxs-lookup"><span data-stu-id="00fb9-153">**Unable to see invoice for the last billing period**</span></span>

<span data-ttu-id="00fb9-154">송장을 볼 수 없는 몇 가지 이유는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-154">Some possible reasons you might not see an invoice:</span></span>

- <span data-ttu-id="00fb9-155">구독에 대 한 월별 신용이 초과 되거나 사용자에 게 무료 평가판이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-155">You have a monthly credit amount with your subscription that you didn't exceed or you have a Free Trial.</span></span> <span data-ttu-id="00fb9-156">금액이 확실 금액을 사용할 때만 생성 되는 송장</span><span class="sxs-lookup"><span data-stu-id="00fb9-156">An invoice is only generated when you owe money</span></span>
- <span data-ttu-id="00fb9-157">Azure에서 구독 한 날 로부터 30 일 미만입니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-157">It's less than 30 days from the day you subscribed to Azure</span></span>
- <span data-ttu-id="00fb9-158">송장이 아직 생성 되지 않았습니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-158">The invoice isn't generated yet.</span></span> <span data-ttu-id="00fb9-159">청구 기간이 끝날 때까지 기다립니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-159">Wait until the end of the billing period</span></span>
- <span data-ttu-id="00fb9-160">계정 관리자가 아닌 경우 이전 송장을 사용 하지 못할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-160">If you're not the Account Administrator, older invoices may not be available to you</span></span>

<span data-ttu-id="00fb9-161">**Azure portal (.pdf)에서 청구서 다운로드**</span><span class="sxs-lookup"><span data-stu-id="00fb9-161">**Download your invoice from Azure portal (.pdf)**</span></span>

- <span data-ttu-id="00fb9-162">[송장에 대 한 액세스 권한이 있는 사용자](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support) 로 Azure Portal의 [구독](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) 페이지에서 구독을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-162">Select your subscription from the [Subscriptions](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) page in Azure portal as [a user with access to invoices](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>
- <span data-ttu-id="00fb9-163">**송장** 선택</span><span class="sxs-lookup"><span data-stu-id="00fb9-163">Select **Invoices**</span></span>
- <span data-ttu-id="00fb9-164">**송장 다운로드** 를 클릭 하 여 PDF 송장의 복사본을 봅니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-164">Click **Download Invoice** to view a copy of your PDF invoice.</span></span> <span data-ttu-id="00fb9-165">**사용할 수 없는** 경우 [마지막 대금 청구 기간에 대 한 송장이 표시 되지 않는 이유](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice) 를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="00fb9-165">If it says **Not available** , see [Why don't I see an invoice for the last billing period?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)</span></span>

<span data-ttu-id="00fb9-166">**전자 메일로 송장 받기 (.pdf)**</span><span class="sxs-lookup"><span data-stu-id="00fb9-166">**Receive your invoice in email (.pdf)**</span></span>

- <span data-ttu-id="00fb9-167">[구독 페이지에서](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) 구독을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-167">Select your subscription from the [Subscriptions](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) page.</span></span> <span data-ttu-id="00fb9-168">**송장을** 클릭 하 고 송장을 전자 메일로 보내기</span><span class="sxs-lookup"><span data-stu-id="00fb9-168">Click **Invoices** then Email my invoice</span></span>
- <span data-ttu-id="00fb9-169">**옵트인** 을 클릭 하 고 사용권 조항에 동의 합니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-169">Click **opt in** and accept the terms.</span></span> <span data-ttu-id="00fb9-170">소유한 각 구독에 대해 옵트인 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-170">You will have to opt in for each subscription you own</span></span>

<span data-ttu-id="00fb9-171">참고: 단계를 수행한 후에는 전자 메일을 받을 수 없는 경우 [프로필의 통신 기본 설정](https://account.windowsazure.com/profile) 에서 전자 메일 주소가 올바른지 확인 하세요.</span><span class="sxs-lookup"><span data-stu-id="00fb9-171">Note: If you don't get an email after following the steps, make sure your email address is correct in the [communication preferences on your profile](https://account.windowsazure.com/profile)</span></span>

<span data-ttu-id="00fb9-172">**Azure portal에서 사용 현황 데이터를 다운로드 합니다.**</span><span class="sxs-lookup"><span data-stu-id="00fb9-172">**Download your usage data from the Azure portal**</span></span>

- <span data-ttu-id="00fb9-173">[계정 관리자로](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa) [Azure 계정 센터](https://account.windowsazure.com/Subscriptions) 에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-173">Sign into the [Azure Account Center](https://account.windowsazure.com/Subscriptions) as the [Account Admin](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)</span></span>
- <span data-ttu-id="00fb9-174">송장 및 사용 현황 정보를 보려는 구독을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-174">Select the subscription for which you want the invoice and usage information</span></span>
- <span data-ttu-id="00fb9-175">**청구 내역** 선택</span><span class="sxs-lookup"><span data-stu-id="00fb9-175">Select **Billing History**</span></span>
- <span data-ttu-id="00fb9-176">추정치를 생성 한 시간에 예상 되는 청구 금액을 보려면 **Current 문 보기** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-176">Select **View Current Statement** to see an estimate of your charges at the time the estimate was generated</span></span>
- <span data-ttu-id="00fb9-177">일별 사용 현황 데이터를 CSV 파일로 다운로드 하려면 **사용 현황 다운로드** 를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="00fb9-177">Select **Download Usage** to download the daily usage data as a CSV file.</span></span> <span data-ttu-id="00fb9-178">두 버전을 사용할 수 있는 경우 버전 2를 다운로드 하세요.</span><span class="sxs-lookup"><span data-stu-id="00fb9-178">If you see two versions available, download version 2</span></span>

<span data-ttu-id="00fb9-179">기타 질문: [예약된 인스턴스 문서 방문](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="00fb9-179">Other questions: [Visit reserved instance docs](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="00fb9-180">**추천 문서**</span><span class="sxs-lookup"><span data-stu-id="00fb9-180">**Recommended Documents**</span></span>

- [<span data-ttu-id="00fb9-181">요금 청구 기본 사항</span><span class="sxs-lookup"><span data-stu-id="00fb9-181">Billing basics</span></span>](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="00fb9-182">예약 된 인스턴스 할인이 적용 되는 방식 이해</span><span class="sxs-lookup"><span data-stu-id="00fb9-182">Understand how the Reserved Instance discount is applied</span></span>](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="00fb9-183">Azure 청구 송장 및 일별 사용 현황 데이터 다운로드 또는 보기</span><span class="sxs-lookup"><span data-stu-id="00fb9-183">Download or view your Azure billing invoice and daily usage data</span></span>](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="00fb9-184">예약 된 인스턴스 할인이 적용 되는 방식 이해</span><span class="sxs-lookup"><span data-stu-id="00fb9-184">Understand how the Reserved Instance discount is applied</span></span>](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="00fb9-185">사용자에 게 요금 청구 구독에 예약 된 인스턴스 사용 이해</span><span class="sxs-lookup"><span data-stu-id="00fb9-185">Understand Reserved Instance usage for your Pay-As-You-Go subscription</span></span>](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="00fb9-186">엔터프라이즈 등록에 대 한 예약 된 인스턴스 사용 이해</span><span class="sxs-lookup"><span data-stu-id="00fb9-186">Understand Reserved Instance usage for your Enterprise enrollment</span></span>](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="00fb9-187">Windows 소프트웨어 비용이 예약 된 인스턴스에 포함 되지 않음</span><span class="sxs-lookup"><span data-stu-id="00fb9-187">Windows software costs not included with Reserved instances</span></span>](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="00fb9-188">파트너의 CSP (중앙 클라우드 솔루션 공급자) 프로그램에 예약 된 인스턴스</span><span class="sxs-lookup"><span data-stu-id="00fb9-188">Reserved Instances in Partner Central Cloud Solution Provider (CSP) program</span></span>](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)