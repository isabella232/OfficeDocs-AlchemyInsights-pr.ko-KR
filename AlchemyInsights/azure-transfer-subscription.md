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
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48840635"
---
# <a name="transfer-azure-billing-ownership"></a>Azure 청구 소유권 이전

전송할 구독이 있는 청구 계정의 관리자로 [Azure 포털](https://portal.azure.com/)에 로그인합니다. 사용자가 관리자인지 확실하지 않거나 관리자가 누구인지 확인해야 하는 경우에는 [계정 청구 관리자 확인](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa)을 참조하세요.

- **비용 관리 + 청구** 검색
- 왼쪽 창에서 **구독** 을 선택합니다. 액세스 권한에 따라 청구 범위를 선택한 후, **구독** 혹은 **Azure 구독** 을 선택해야할 수 있습니다.
- 이전할 구독의 **청구 소유권 이전** 을 선택합니다.
- 구독에 대한 새 소유자가 될 계정의 청구 관리자인 사용자의 전자 메일 주소를 입력한 다음 **이전 요청 보내기** 를 선택합니다.
- 사용자는 이전 요청을 검토하는 지침이 포함된 전자 메일을 받습니다. 이전 요청을 승인하려면 사용자는 전자 메일에서 링크를 선택하고 지침을 따릅니다.

**참고** : 구독의 대금 청구 소유권을 다른 Azure AD 테넌트에 있는 사용자의 계정에 이전하는 경우, 구독에서 리소스를 관리하기 위한 모든 [RBAC(역할 기반 액세스 제어)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) 할당이 영구적으로 제거됩니다. 새 소유자만 구독에서 리소스를 관리하는 데 액세스할 수 있습니다. 자세한 내용은 [다른 Azure AD 테넌트에 있는 사용자에게 구독 이전](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)을 참조하세요.

**추천 문서**

- [Azure 구독의 청구 소유권을 다른 계정으로 이전](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Azure 구독의 청구 소유권 이전에 대한 정보](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Visual Studio, Microsoft 파트너 네트워크 (MPN) 및 종량제 개발/테스트 구독의 이전](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [소유권 이전 FAQ](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [소유권 이전 문제 해결](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
