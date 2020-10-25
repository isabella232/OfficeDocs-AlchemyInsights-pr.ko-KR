---
title: 구독/계정 사용 안 함 규칙
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
- "9003559"
- "6676"
ms.openlocfilehash: 6a350c6bca18306e64f647cfa3a7f14fa204109b
ms.sourcegitcommit: 9626d39e5891f83774ba31574a00b0bae92ad442
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/24/2020
ms.locfileid: "48755599"
---
# <a name="azure-subscription-disabled"></a>Azure 구독 사용 안 함

크레딧이 만료 되었거나, 지출 한도를 초과 했거나, 신용 카드 제한에 도달 하거나, 계정 관리자가 구독을 취소 했기 때문에 Azure 구독을 사용 하지 않도록 설정할 수 있습니다. 구독을 다시 사용 하도록 설정 하는 방법에 대해서는 아래를 참조 하세요. 자세한 정보: [Azure 구독 다시 활성화](https://docs.microsoft.com/azure/billing/billing-subscription-become-disable?WT.mc_id=Portal-Microsoft_Azure_Support)

**Azure 구독을 다시 사용 하도록 설정 (구독이 실수로 취소 됨)** [계정 관리자](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa) 는 계정 센터에서 취소 된 비용 청구 구독을 다시 활성화할 수 있습니다.

1. [계정 센터](https://account.windowsazure.com/Subscriptions)에 로그인 합니다.
2. 취소 된 구독을 선택 합니다. **다시 활성화**를 클릭 합니다.

다른 구독 유형에 대해서는 [지원 서비스에 문의](https://portal.azure.com/?#blade/Microsoft_Azure_Support/HelpAndSupportBlade) 하 여 구독을 다시 활성화 해야 합니다.

**만료 된 신용 카드**

**Azure 무료 계정**에 등록할 때 무료 평가판 구독을 사용 하 여 30 일에서의 azure 제작진 및 12 개월 무료 서비스에 $200를 제공 합니다. 30 일이 지나면 Azure에서 구독을 사용 하지 않도록 설정 합니다. 구독에 포함 된 크레딧 및 무료 서비스를 초과 하 여 사용을 방지 하기 위해 구독을 사용 하지 않도록 설정 되었습니다. Azure 서비스를 계속 사용 하려면 구독을 [업그레이드](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)해야 합니다. 업그레이드 후에도 구독은 12 개월 동안 무료 서비스에 액세스할 수 있습니다. 무료 사용 가능 서비스 및 수량 이상의 사용량을 지불 해야 합니다.  
자세한 내용은 [만료 된 신용 카드](https://docs.microsoft.com/azure/billing/billing-subscription-become-disable?WT.mc_id=Portal-Microsoft_Azure_Support#your-credit-is-expired) 를 확인 하세요.

**지출 제한 도달**

사용량이 지출 제한에 도달 하면 Azure는 해당 청구 기간의 나머지 기간 동안 구독을 사용 하지 않도록 설정 합니다. 구독에 포함 된 신용에 대해 실수로 요금 청구를 방지 하기 위해 구독이 사용 되지 않도록 설정 되었습니다. 지출 한도를 제거 하려면 [Azure 지출 제한을](https://docs.microsoft.com/azure/cost-management-billing/manage/spending-limit?WT.mc_id=Portal-Microsoft_Azure_Support)참조 하세요.  
자세한 정보: [지출 제한에 도달 함](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled?WT.mc_id=Portal-Microsoft_Azure_Support#you-reached-your-spending-limit)

**청구서 기한**

지난 기한 잔액을 확인 하려면 [azure에서 전자 메일을 가져온 후 azure 구독에 대 한 기한이 지난 기한 문제 해결](https://docs.microsoft.com/azure/billing/billing-azure-subscription-past-due-balance?WT.mc_id=Portal-Microsoft_Azure_Support)을 참조 하세요.

**청구 금액이 신용 카드 한도를 초과 함**

이 문제를 해결 하려면 [다른 신용 카드로 전환](https://docs.microsoft.com/azure/billing/billing-how-to-change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support)합니다. 또는 비즈니스를 대표 하는 경우 [송장 별로 결제로 전환할](https://docs.microsoft.com/azure/billing/billing-how-to-pay-by-invoice?WT.mc_id=Portal-Microsoft_Azure_Support)수 있습니다.

**참고**: 새 구독 기념일 (SA) 날짜는 다시 사용 하도록 설정 된 구독에 할당 됩니다. 구독이 일시 중단 된 일 수 (간격)로, 원래 SA 날짜에 추가 됩니다. 모든 기념일이 29 일, 30 일 또는 31이 되 면 SA 날짜가 다음 달의 1 일로 설정 됩니다.  
예제:

- 원래 구독 기념일은 25입니다.
- 구독이 10/3에 일시 중단 되 고 10/9에서 다시 사용 하도록 설정 되었습니다.
- 구독을 사용할 수 없도록 6 일 (간격 6),
- 그러면 간격이 원래 SA에 추가 되 고 합계가 새 SA 날짜 (25 + 6 = 31)가 됩니다. 

**참고**:이 예에서 SA 날짜는 이제 28 보다 크므로 새 SA 날짜는 다음 달의 1 일이 됩니다.

**권장 문서**

- [구독 전환](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)  
- [구독 취소](https://docs.microsoft.com/azure/billing/billing-how-to-cancel-azure-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)  
- [Azure Marketplace](https://azuremarketplace.microsoft.com/marketplace/?source=datamarket)
- [계정 관리자](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa) 찾기
- [Azure 구독이 사용 하지 않도록 설정 되 면 어떻게 하나요?](https://docs.microsoft.com/azure/billing/billing-subscription-become-disable/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure 지출 한도](https://docs.microsoft.com/azure/cost-management-billing/manage/spending-limit?WT.mc_id=Portal-Microsoft_Azure_Support)
