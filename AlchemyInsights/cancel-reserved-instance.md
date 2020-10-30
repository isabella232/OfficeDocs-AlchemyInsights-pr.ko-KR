---
title: 예약 취소
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
- "9003552"
- "6817"
ms.openlocfilehash: 04875e33f07c6d0a4306b3579ef81f2d28c7f506
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/28/2020
ms.locfileid: "48791480"
---
# <a name="cancelling-reservation"></a><span data-ttu-id="77859-102">예약 취소</span><span class="sxs-lookup"><span data-stu-id="77859-102">Cancelling Reservation</span></span>

- <span data-ttu-id="77859-103">**셀프 서비스:**[Azure 포털](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)을 사용하여 직접 예약된 인스턴스를 취소하거나 교환할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="77859-103">**Self-service:** You can cancel or exchange a reserved instance yourself using [Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade).</span></span> <span data-ttu-id="77859-104">예약을 선택하고 환불 또는 교환을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="77859-104">Select the reservation and click on refund or exchange.</span></span> <span data-ttu-id="77859-105">교환 또는 환불을 하려면 예약 순서에 대한 소유자 액세스 권한이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="77859-105">Note that you must have owner access on the Reservation Order to exchange or refund.</span></span> <span data-ttu-id="77859-106">예약으로만 액세스하는 경우에는 환불이나 교환 처리를 진행할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="77859-106">Access to only the Reservation will not let you proceed with refund or exchange.</span></span> <span data-ttu-id="77859-107">예약 순서 소유자에게 예약 순서에 대한 소유자 액세스 권한을 요청합니다.</span><span class="sxs-lookup"><span data-stu-id="77859-107">Ask the Reservation Order owner to give you owner access to the Reservation Order</span></span>
- <span data-ttu-id="77859-108">**교환 정책:** 동일한 유형의 다른 예약으로 교환할 수 있습니다. 예약 변경에 대한 **벌금은 없습니다** .</span><span class="sxs-lookup"><span data-stu-id="77859-108">**Exchange policy:** You can exchange a reservation for another reservation of the same type – there are **no penalties** on reservation exchange.</span></span> <span data-ttu-id="77859-109">새 예약을 사용하는 총 약정 금액은 교환되는 예약의 환불 금액과 차후의 월간 지불액(해당하는 경우)의 합계를 초과해야 합니다. </span><span class="sxs-lookup"><span data-stu-id="77859-109">The total commitment with new reservation should be greater than the sum of exchanged reservation’s refund amount and the future monthly payments (if applicable)</span></span>
- <span data-ttu-id="77859-110">**환불 정책:** 환불 금액의 합계와 취소된 차후의 지불액은 12개월의 상환 기간에 $50,000을 초과할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="77859-110">**Refund policy:** Sum of refund and the cancelled future payments cannot exceed $50,000 USD in a 12-month rolling window.</span></span> <span data-ttu-id="77859-111">**현재는 환불에 대한 벌금이 없지만** 차후에는 청구할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="77859-111">We are **currently not charging any penalty** on refunds but could charge it on future refunds</span></span>  
    <span data-ttu-id="77859-112">**예외 사항:** 셀프 서비스 교환 및 취소 기능은 미국 정부 기업 계약 고객에게는 제공되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="77859-112">**Exceptions:** Self-service exchange and cancel capability isn't available for US Government Enterprise Agreement customers</span></span>
- <span data-ttu-id="77859-113">**API / PS / CLI** 지원은 취소 및 환불에 대해서는 제공되지 않음 [Azure 예약에 대한 셀프 서비스 교환 및 환불](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="77859-113">**API / PS / CLI** support is not available for cancellation and refunds [Self-service exchanges and refunds for Azure Reservations](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>
- <span data-ttu-id="77859-114">셀프 서비스 교환 및 취소 기능은 미국 정부 기업 계약 고객에게는 제공되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="77859-114">Self-service exchange and cancel capability isn't available for US Government Enterprise Agreement customers.</span></span> <span data-ttu-id="77859-115">용량제를 포함하고 CSP가 지원되는 기타 미국 정부 기관용 구독 유형</span><span class="sxs-lookup"><span data-stu-id="77859-115">Other US Government subscription types including Pay-As-You-Go and CSP are supported</span></span>

<span data-ttu-id="77859-116">자세한 정보: [반환 및 교환 트랜잭션을 처리 하는 방법](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)</span><span class="sxs-lookup"><span data-stu-id="77859-116">Learn more : [How return and exchange transactions are processed](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)</span></span>  
<span data-ttu-id="77859-117">자세한 정보: [교환 및 환불 정책](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)</span><span class="sxs-lookup"><span data-stu-id="77859-117">Learn more : [Exchange and Refund policies](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)</span></span>  
<span data-ttu-id="77859-118">기타 질문: [예약된 인스턴스 문서 방문](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="77859-118">Other questions: [Visit reserved instance docs](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="77859-119">**기존에 예약된 인스턴스 교환(셀프 서비스)**</span><span class="sxs-lookup"><span data-stu-id="77859-119">**Exchange an existing reserved instance (Self-service)**</span></span>

<span data-ttu-id="77859-120">동일한 유형의 다른 예약으로 예약을 교환할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="77859-120">You can exchange a reservation for another reservation of the same type.</span></span> <span data-ttu-id="77859-121">더 이상 필요하지 않은 경우 연간 최대 $50,000 USD까지의 예약을 환불할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="77859-121">You can also refund a reservation, up to $50,000 USD per year, if you no longer need it.</span></span> <span data-ttu-id="77859-122">셀프 서비스 교환 및 취소 기능은 미국 정부 기업 계약 고객에게는 제공되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="77859-122">Self-service exchange and cancel capability isn't available for US Government Enterprise Agreement customers.</span></span> <span data-ttu-id="77859-123">용량제를 포함하고 CSP가 지원되는 기타 미국 정부 기관용 구독 유형입니다.</span><span class="sxs-lookup"><span data-stu-id="77859-123">Other US Government subscription types including Pay-As-You-Go and CSP are supported.</span></span> <span data-ttu-id="77859-124">기존 예약을 교환하거나 환불하려면 예약 순서에 대한 소유자 액세스 권한이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="77859-124">You must have owner access on the Reservation Order to exchange or refund an existing reservation.</span></span>

<span data-ttu-id="77859-125">다음 단계는 거래를 완료하기 위한 절차를 안내합니다.</span><span class="sxs-lookup"><span data-stu-id="77859-125">The following steps will guide on the procedure to complete the transaction</span></span>

1. <span data-ttu-id="77859-126">[Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="77859-126">Log in to your [Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade).</span></span> <span data-ttu-id="77859-127">환불하려는 예약을 선택하고 **교환** 을 클릭</span><span class="sxs-lookup"><span data-stu-id="77859-127">Select the reservations that you want to refund and click **Exchange**</span></span>
2. <span data-ttu-id="77859-128">구입하려는 VM 제품을 선택하고 수량을 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="77859-128">Select the VM product that you want to purchase and type a quantity.</span></span> <span data-ttu-id="77859-129">새 구매 총액이 반품 총액을 초과하는지 확인 [구매하기 전에 올바른 사이즈를 결정](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)</span><span class="sxs-lookup"><span data-stu-id="77859-129">Make sure that the new purchase total is more than the return total [Determine the right size before you purchase](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)</span></span>
3. <span data-ttu-id="77859-130">트랜잭션 검토 및 완료</span><span class="sxs-lookup"><span data-stu-id="77859-130">Review and complete the transaction</span></span>

<span data-ttu-id="77859-131">**예약된 인스턴스에 대한 환불**</span><span class="sxs-lookup"><span data-stu-id="77859-131">**Refund for a reserved instance**</span></span>

<span data-ttu-id="77859-132">예약을 환불하려면 **예약 세부 정보** 로 이동하여 **환불** 을 클릭</span><span class="sxs-lookup"><span data-stu-id="77859-132">To refund a reservation, go to **Reservation Details** and click **Refund**</span></span>

<span data-ttu-id="77859-133">**비례 배분 환불:**</span><span class="sxs-lookup"><span data-stu-id="77859-133">**Pro-rated refund:**</span></span>

<span data-ttu-id="77859-134">**환불 및 교환에 대한 비례 배분 및 최소 요구 사항 예시**</span><span class="sxs-lookup"><span data-stu-id="77859-134">**Pro-ration and minimum requirement examples for refund and exchange**</span></span>  
<span data-ttu-id="77859-135">선행 예약 예시:</span><span class="sxs-lookup"><span data-stu-id="77859-135">Upfront reservation example:</span></span>

- <span data-ttu-id="77859-136">1월 1일에 1년의 기간을 $120에 구매</span><span class="sxs-lookup"><span data-stu-id="77859-136">You purchase a one-year term RI for $120 on January 1</span></span>
- <span data-ttu-id="77859-137">4월 7일에 이 예약을 환불 혹은 교환하고자 함</span><span class="sxs-lookup"><span data-stu-id="77859-137">On April 7th you want to refund or exchange this reservation</span></span>
- <span data-ttu-id="77859-138">이 예약은 97일간에 제공되었기 때문에 (1-97/365) \* $120을 환불 받습니다.</span><span class="sxs-lookup"><span data-stu-id="77859-138">Since the reservation has been live for 97 days, you will get (1-97/365) \* $120 back.</span></span> <span data-ttu-id="77859-139">(즉, $88.1).</span><span class="sxs-lookup"><span data-stu-id="77859-139">(i.e. $88.1).</span></span> <span data-ttu-id="77859-140">현재 환불에 대한 벌금은 없습니다.</span><span class="sxs-lookup"><span data-stu-id="77859-140">There is currently no penalty on refunds</span></span>
- <span data-ttu-id="77859-141">교환할 경우, 새 구매는 $88.1을 초과해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="77859-141">If exchanging, your new purchase should be greater than $88.1</span></span>
- <span data-ttu-id="77859-142">현재 환불에 대한 벌금은 없습니다.</span><span class="sxs-lookup"><span data-stu-id="77859-142">There is no penalty on refunds currently</span></span>

<span data-ttu-id="77859-143">**청구 계획 예약 예시:**</span><span class="sxs-lookup"><span data-stu-id="77859-143">**Billing plan reservation example:**</span></span>

- <span data-ttu-id="77859-144">1년 기간의 RI를 월간 $10에 구매</span><span class="sxs-lookup"><span data-stu-id="77859-144">You purchase a one-year term RI for $10 per month</span></span>
- <span data-ttu-id="77859-145">4월 7일에 이 예약을 환불 혹은 교환하고자 함</span><span class="sxs-lookup"><span data-stu-id="77859-145">On April 7th you want to refund or exchange this reservation</span></span>
- <span data-ttu-id="77859-146">마지막 결재가 7일 전에 처리되었으므로 (1-7/31) \* $10을 환불 받습니다.</span><span class="sxs-lookup"><span data-stu-id="77859-146">Since the last payment happened 7 days, you will get (1-7/31) \* $10 back.</span></span> <span data-ttu-id="77859-147">(즉, $7.74)</span><span class="sxs-lookup"><span data-stu-id="77859-147">(i.e. $7.74)</span></span>
- <span data-ttu-id="77859-148">이후의 결제는 $80입니다.</span><span class="sxs-lookup"><span data-stu-id="77859-148">The future payments cancelled are $ 80.</span></span> <span data-ttu-id="77859-149">현재 환불에 대한 벌금은 없습니다.</span><span class="sxs-lookup"><span data-stu-id="77859-149">There is currently no penalty on refunds</span></span>
- <span data-ttu-id="77859-150">이 취소는 귀하의 환불 한도 $50,000에서 $87.74를 차감합니다.</span><span class="sxs-lookup"><span data-stu-id="77859-150">This cancellation will deduct $87.74 from you’re the $50,000 refund limit</span></span>
- <span data-ttu-id="77859-151">교환할 경우, 신규 구매의 총액은 $87.74을 초과해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="77859-151">If exchanging, the total value of new purchase should be greater than $87.74</span></span>

<span data-ttu-id="77859-152">**추천 문서**</span><span class="sxs-lookup"><span data-stu-id="77859-152">**Recommended Documents**</span></span>

- [<span data-ttu-id="77859-153">반품 및 교환 트랜잭션을 처리하는 방법</span><span class="sxs-lookup"><span data-stu-id="77859-153">How return and exchange transactions are processed</span></span>](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [<span data-ttu-id="77859-154">교환 및 환불 정책</span><span class="sxs-lookup"><span data-stu-id="77859-154">Exchange and Refund policies</span></span>](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)