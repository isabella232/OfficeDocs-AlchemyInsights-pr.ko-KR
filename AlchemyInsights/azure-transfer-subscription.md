---
title: Azure 청구 소유권 이전
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
- "6849"
ms.openlocfilehash: 454ce626862bb4a2361abccd92ad0099b534388c
ms.sourcegitcommit: 059ad2936788266ea9714ec8c66d407d7261aeb6
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/29/2020
ms.locfileid: "49736884"
---
# <a name="transfer-azure-billing-ownership"></a>Azure 청구 소유권 이전

전송할 구독이 있는 청구 계정의 관리자로 [Azure portal](https://portal.azure.com/)에 로그인합니다. 사용자가 관리자인지 확실하지 않거나 관리자가 누구인지 확인해야 하는 경우에는 [계정 청구 관리자 확인](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa)을 참조하세요.

1. _비용 관리 + 청구_ 검색
1. 왼쪽 창에서 **구독** 을 선택합니다. 액세스 권한에 따라 청구 범위를 선택한 후, **구독** 혹은 **Azure 구독** 을 선택해야할 수 있습니다.
1. 이전할 구독의 **청구 소유권 이전** 을 선택합니다.
1. 구독에 대한 새 소유자가 될 계정의 청구 관리자인 사용자의 전자 메일 주소를 입력한 다음 **이전 요청 보내기** 를 선택합니다.
1. 사용자는 이전 요청을 검토하는 지침이 포함된 전자 메일을 받습니다. 이전 요청을 승인하려면 사용자는 전자 메일에서 링크를 선택하고 지침을 따릅니다.

구독의 대금 청구 소유권을 다른 Azure AD 테넌트에 있는 사용자의 계정에 이전하는 경우, 구독에서 리소스를 관리하기 위한 모든 [RBAC(역할 기반 액세스 제어)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) 할당이 영구적으로 제거된다는 점에 유의하세요. 새 소유자만 구독에서 리소스를 관리하는 데 액세스할 수 있습니다. 구독에 대한 디렉터리를 변경하는 방법에 대한 자세한 내용은 [다른 Azure AD 테넌트에 있는 사용자에게 구독 이전](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)을 참조하세요.

_**송장에 대 한 중요한 영향**_: Azure 구독에 대한 청구 소유권을 이전한 경우에는 요금이 비례배분됩니다. 다음 방법에 따라 송장에 액세스할 수 있습니다.  

1.  [송장에 대한 액세스 권한이 있는 사용자](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)로 Azure 포털의  [구독 페이지](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) 에서 구독을 선택한 다음,  **송장** 을 선택합니다.
1. PDF 송장의 복사본을 표시하려면  **송장 다운로드** 를 클릭합니다.  _사용할 수 없음_ 이 표시되는 경우,  [마지막 청구 기간에 대한 송장이 표시되지 않는 이유](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)를 참조하세요.
1. **청구 기간** 을 클릭하여 일별 사용 현황을 볼 수 있습니다. 송장 PDF 및 상세한 일별 사용 현황 파일(.CSV) 복사본을 받으려면 다음을 참조하세요. 자세한 내용은 [송장 및 사용 현황 데이터 가져오기](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)를 참조하세요.

**추천 문서**

- [Azure 구독의 청구 소유권을 다른 계정으로 이전](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Azure 구독의 청구 소유권 이전에 대한 정보](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Visual Studio, Microsoft 파트너 네트워크 (MPN) 및 종량제 개발/테스트 구독의 이전](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [소유권 이전 FAQ](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [소유권 이전 문제 해결](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
