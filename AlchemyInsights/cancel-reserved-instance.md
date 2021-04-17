---
title: 예약 취소
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003552"
- "6817"
ms.openlocfilehash: 6b27344b43aa5c20d64d148ff164be805f3b5ef8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819698"
---
# <a name="cancelling-reservation"></a>예약 취소

- **셀프 서비스:**[Azure 포털](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)을 사용하여 직접 예약된 인스턴스를 취소하거나 교환할 수 있습니다. 예약을 선택하고 환불 또는 교환을 클릭합니다. 교환 또는 환불을 하려면 예약 순서에 대한 소유자 액세스 권한이 있어야 합니다. 예약으로만 액세스하는 경우에는 환불이나 교환 처리를 진행할 수 없습니다. 예약 순서 소유자에게 예약 순서에 대한 소유자 액세스 권한을 요청합니다.
- **교환 정책:** 동일한 유형의 다른 예약으로 교환할 수 있습니다. 예약 변경에 대한 **벌금은 없습니다**. 새 예약을 사용하는 총 약정 금액은 교환되는 예약의 환불 금액과 차후의 월간 지불액(해당하는 경우)의 합계를 초과해야 합니다. 
- **환불 정책:** 환불 금액의 합계와 취소된 차후의 지불액은 12개월의 상환 기간에 $50,000을 초과할 수 없습니다. **현재는 환불에 대한 벌금이 없지만** 차후에는 청구할 수 있습니다.  
    **예외 사항:** 셀프 서비스 교환 및 취소 기능은 미국 정부 기업 계약 고객에게는 제공되지 않습니다.
- **API / PS / CLI** 지원은 취소 및 환불에 대해서는 제공되지 않음 [Azure 예약에 대한 셀프 서비스 교환 및 환불](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- 셀프 서비스 교환 및 취소 기능은 미국 정부 기업 계약 고객에게는 제공되지 않습니다. 용량제를 포함하고 CSP가 지원되는 기타 미국 정부 기관용 구독 유형

자세한 정보: [반환 및 교환 트랜잭션을 처리 하는 방법](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
자세한 정보: [교환 및 환불 정책](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
기타 질문: [예약된 인스턴스 문서 방문](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**기존에 예약된 인스턴스 교환(셀프 서비스)**

동일한 유형의 다른 예약으로 예약을 교환할 수 있습니다. 더 이상 필요하지 않은 경우 연간 최대 $50,000 USD까지의 예약을 환불할 수도 있습니다. 셀프 서비스 교환 및 취소 기능은 미국 정부 기업 계약 고객에게는 제공되지 않습니다. 용량제를 포함하고 CSP가 지원되는 기타 미국 정부 기관용 구독 유형입니다. 기존 예약을 교환하거나 환불하려면 예약 순서에 대한 소유자 액세스 권한이 있어야 합니다.

다음 단계는 거래를 완료하기 위한 절차를 안내합니다.

1. [Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)에 로그인합니다. 환불하려는 예약을 선택하고 **교환** 을 클릭
2. 구입하려는 VM 제품을 선택하고 수량을 입력합니다. 새 구매 총액이 반품 총액을 초과하는지 확인 [구매하기 전에 올바른 사이즈를 결정](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. 트랜잭션 검토 및 완료

**예약된 인스턴스에 대한 환불**

예약을 환불하려면 **예약 세부 정보** 로 이동하여 **환불** 을 클릭

**비례 배분 환불:**

**환불 및 교환에 대한 비례 배분 및 최소 요구 사항 예시**  
선행 예약 예시:

- 1월 1일에 1년의 기간을 $120에 구매
- 4월 7일에 이 예약을 환불 혹은 교환하고자 함
- 이 예약은 97일간에 제공되었기 때문에 (1-97/365) * $120을 환불 받습니다. (즉, $88.1). 현재 환불에 대한 벌금은 없습니다.
- 교환할 경우, 새 구매는 $88.1을 초과해야 합니다.
- 현재 환불에 대한 벌금은 없습니다.

**청구 계획 예약 예시:**

- 1년 기간의 RI를 월간 $10에 구매
- 4월 7일에 이 예약을 환불 혹은 교환하고자 함
- 마지막 결재가 7일 전에 처리되었으므로 (1-7/31) * $10을 환불 받습니다. (즉, $7.74)
- 이후의 결제는 $80입니다. 현재 환불에 대한 벌금은 없습니다.
- 이 취소는 귀하의 환불 한도 $50,000에서 $87.74를 차감합니다.
- 교환할 경우, 신규 구매의 총액은 $87.74을 초과해야 합니다.

**추천 문서**

- [반품 및 교환 트랜잭션을 처리하는 방법](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [교환 및 환불 정책](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)