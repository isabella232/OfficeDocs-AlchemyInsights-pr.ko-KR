---
title: 예약된 인스턴스 구입에 대한 청구
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 00565470de388165e64c45879c22fd5064b4adc695151edaf58878f38a481ff2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104026"
---
# <a name="billing-for-reserved-instance-purchase"></a>예약된 인스턴스 구입에 대한 청구

예약된 인스턴스 구입은 구입 시 선택하는 구독과 연결된 결제 방법으로 요금이 청구됩니다. 구독 유형은 엔터프라이즈 계약(제품 번호: MS-AZR-0017P), 종량제(제품 번호: MS-AZR-0003P), Microsoft 고객 계약이나 CSP여야 합니다.

- 엔터프라이즈 구독의 경우, 요금은 등록자의 금액 약정 잔액에서 공제되거나 초과 사용 기간으로 부과됩니다.
- 종량제 구독의 경우 구독에 대한 신용 카드 또는 청구서 지불 방법으로 요금이 청구됩니다.

**예약 취소**

- **셀프 서비스:**[Azure 포털](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)을 사용하여 직접 예약된 인스턴스를 취소하거나 교환할 수 있습니다. 예약을 선택하고 환불 또는 교환을 클릭합니다. 교환 또는 환불을 하려면 예약 순서에 대한 소유자 액세스 권한이 있어야 합니다. 예약으로만 액세스하는 경우에는 환불이나 교환 처리를 진행할 수 없습니다. 예약 순서 소유자에게 예약 순서에 대한 소유자 액세스 권한을 요청합니다.
- **교환 정책:** 동일한 유형의 다른 예약으로 교환할 수 있습니다. 예약 변경에 대한 **벌금은 없습니다**. 새 예약을 사용하는 총 약정 금액은 교환되는 예약의 환불 금액과 차후의 월간 지불액(해당하는 경우)의 합계를 초과해야 합니다. 
- **환불 정책:** 환불 금액의 합계와 취소된 차후의 지불액은 12개월의 상환 기간에 $50,000을 초과할 수 없습니다. **현재는 환불에 대한 벌금이 없지만** 차후에는 청구할 수 있습니다.

**예외 사항:** 셀프 서비스 교환 및 취소 기능은 미국 정부 기업 계약 고객에게는 제공되지 않습니다.

- **API / PS / CLI** 지원은 취소 및 환불에 대해서는 제공되지 않음 [Azure 예약에 대한 셀프 서비스 교환 및 환불](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- 셀프 서비스 교환 및 취소 기능은 미국 정부 기업 계약 고객에게는 제공되지 않습니다. 용량제를 포함하고 CSP가 지원되는 기타 미국 정부 기관용 구독 유형

자세한 정보: [반환 및 교환](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) 트랜잭션 처리 방법 자세한 정보 : Exchange 및 환불 [정책](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) 기타 질문: 예약된 인스턴스 [docs 방문](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**기존에 예약된 인스턴스 교환(셀프 서비스)**

동일한 유형의 다른 예약으로 예약을 교환할 수 있습니다. 더 이상 필요하지 않은 경우 연간 최대 $50,000 USD까지의 예약을 환불할 수도 있습니다. 셀프 서비스 교환 및 취소 기능은 미국 정부 기업 계약 고객에게는 제공되지 않습니다. 용량제를 포함하고 CSP가 지원되는 기타 미국 정부 기관용 구독 유형입니다. 기존 예약을 교환하거나 환불하려면 예약 순서에 대한 소유자 액세스 권한이 있어야 합니다.

다음 단계는 거래를 완료하기 위한 절차를 안내합니다.

1.Azure [Portal에 로그인합니다.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) 환불할 예약을 선택하고 Exchange  2.구매할 VM 제품을 선택하고 수량을 입력합니다. 새 구매 총액이 반환 총액보다 큰지 확인 구매하기 전에 올바른 [크기를 결정해야 합니다.](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3.거래 검토 및 완료

**예약된 인스턴스에 대한 환불**

예약을 환불하려면 **예약 세부 정보** 로 이동하여 **환불** 을 클릭

**비례 배분 환불:**

**Pro 및** 교환에 대한 최소 요구 사항 예 선행 예약 예시:

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

**마지막 청구 기간에 대한 송장을 볼 수 없습니다.**

가능한 몇 가지 이유로 송장이 표시되지 않을 수 있습니다.

- 구독에서 초과하지 않은 월별 크레딧 금액이 있는 경우 또는 무료 평가판이 있습니다. 송장은 돈을 지불할 때만 생성됩니다.
- Azure에 구독한 날로부터 30일 미만
- 송장이 아직 생성되지 않았습니다. 청구 기간이 끝날 때까지 기다림
- 계정 관리자가 아닌 경우 이전 송장을 사용할 수 없는 것일 수 있습니다.

**Azure Portal에서 송장 다운로드(.pdf)**

- 송장에 액세스할 [](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) 수 있는 사용자로 Azure Portal의 구독 페이지에서 구독 [선택](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- 송장 **선택**
- PDF 송장의 복사본을 표시하려면 **송장 다운로드** 를 클릭합니다. **사용할 수 없음** 이 표시되는 경우, [마지막 청구 기간에 대한 송장이 표시되지 않는 이유](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)를 참조하세요.

**전자 메일로 송장 받기(.pdf)**

- 구독 페이지에서 [구독을](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) 선택합니다. Click **Invoices** then Email my invoice
- **옵트인(opt in)을** 클릭하고 사용 약관에 동의합니다. 소유한 각 구독에 대해 옵트인해야 합니다.

참고: 단계를 수행한 후 전자 메일을 받을 수 없는 경우 프로필의 통신 기본 설정에서 전자 메일 주소가 [올바른지 확인합니다.](https://account.windowsazure.com/profile)

**Azure Portal에서 사용 현황 데이터 다운로드**

- 계정 관리자로 [Azure 계정](https://account.windowsazure.com/Subscriptions) [센터에 로그인](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- 송장 및 사용 정보를 원하는 구독 선택
- 청구 **내역 선택**
- 예상 **요금이 생성된** 시간의 예상 요금을 확인하려면 현재 문 보기를 선택합니다.
- 사용 **현황 다운로드를 선택하여** 일별 사용 현황 데이터를 CSV 파일로 다운로드합니다. 사용 가능한 두 버전이 표시되는 경우 버전 2 다운로드

기타 질문: [예약된 인스턴스 문서 방문](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**추천 문서**

- [청구 기본](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [예약 인스턴스 할인이 적용되는 방식 이해](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure 청구 송장 및 일별 사용 현황 데이터 다운로드 또는 보기](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [예약 인스턴스 할인이 적용되는 방식 이해](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Pay-As-Go 구독에 대한 예약된 인스턴스 사용 이해](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [사용자 등록에 대한 예약된 Enterprise 이해](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows 인스턴스에 포함되지 않은 소프트웨어 비용](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [CSP(Partner Central 클라우드 솔루션 공급자)의 예약된 인스턴스](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)