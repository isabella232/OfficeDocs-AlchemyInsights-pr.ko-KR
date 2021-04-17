---
title: 지원되는 구독 유형
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
- "9003560"
- "6675"
ms.openlocfilehash: dcf5855bff8725ea746196c1f07d689ce1797f8c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820688"
---
# <a name="supported-subscription-types"></a>지원되는 구독 유형

지원되는 구독 유형을 검토하여 계속 진행하세요.

[지원되는 구독 유형](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**대금 청구 소유권 이전**

이전하려는 구독이 있는 청구 계정의 [계정 관리자](https://ms.portal.azure.com/)로서 Azure Portal

- **비용 관리 + 청구** 검색 왼쪽 창에서 **구독** 을 선택합니다. 액세스 권한에 따라 청구 범위를 선택한 후, **구독** 혹은 **Azure 구독** 을 선택해야할 수 있습니다.
- 이전할 구독의 청구 소유권 이전을 선택합니다.
- 구독에 대한 새 소유자가 될 계정의 청구 관리자인 사용자의 전자 메일 주소를 입력한 다음 **이전 요청 보내기** 를 선택합니다.
- 사용자는 이전 요청을 검토하는 지침이 포함된 전자 메일을 받습니다. 이전 요청을 승인하려면 사용자는 전자 메일에서 링크를 선택하고 지침을 따릅니다.

참고: 구독의 대금 청구 소유권을 다른 Azure AD 테넌트에 있는 사용자의 계정에 이전하는 경우, 구독에서 리소스를 관리하기 위한 모든 [RBAC(역할 기반 액세스 제어)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) 할당이 영구적으로 제거됩니다. 새 소유자만 구독에서 리소스를 관리하는 데 액세스할 수 있습니다. 자세한 내용은 [다른 Azure AD 테넌트에 있는 사용자에게 구독 이전](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)을 참조하세요.

**구독의 소유권 이전**

구독 소유권 이전 시 필수 구성 요소인 구독에서 리소스를 관리하기 위한 RBAC(역할 기반 액세스 제어)에 대한 액세스 권한을 잃게 됩니다. 기존 구독을 테넌트에 추가하는 방법에 대한 자세한 내용은 [Azure 구독을 Azure Active Directory에 연결 또는 추가](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support)를 참조하세요.

- 현재 대금 청구 주기에 기존 미납 금액이 있는 구독을 이전하면 새 계정의 새 결제 방법으로 이전되지 않습니다. 새 계정에서 사용자가 사용할 수 있는 유일한 정보는 구독에 대 한 마지막 월간 비용입니다. 나머지 사용 및 청구 기록은 구독과 함께 전송 되지 않습니다.
- 엔터프라이즈 규약 (EA) 구독의 대금 청구 소유권 전송은 현재 엔터프라이즈 규약 포털 에서만 지원 됩니다.
- Visual Studio, BizSpark, Microsoft 파트너 네트워크와 같은 신용을 바탕으로 한 구독을 새 사용자에게 이전하려면 Visual Studio/Microsoft 파트너 네트워크 라이선스가 있어야 이전 요청을 수락할 수 있습니다.
- 가상 컴퓨터, 디스크 및 웹 사이트와 같은 모든 리소스는 새 계정으로 이전됩니다. 다음 리소스는 테넌트 간의 구독 이전 시 영향을 받을 수 있습니다.

**Azure AD 도메인 서비스**

Azure Key Vault

- 특히 고객이 Azure Active Directory 관련 인증을 사용하는 경우, [SQL 관련 사용자 및 데이터베이스](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support)가 영향을 받을 수 있습니다.
- Azure Active Directory 인증을 사용하여 구성된 **App Services** 가 영향을 받을 수 있습니다.
- Azure 구독에 연결된 **Visual Studio Team** Services 계정은 연결된 Azure 구독이 취소될 때 일시적으로 액세스 권한을 잃을 수 있습니다.

**추천 문서**

대금 청구 소유권을 수락한 후의 단계:

- 대금 청구 소유권을 유지하되 구독의 유형을 변경하려면 [Azure 구독을 다른 플랜으로 전환](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)을 참조하세요.
- [Visual Studio, Microsoft 파트너 네트워크 (MPN) 및 종량제 개발/테스트 구독의 이전](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [EA(엔터프라이즈 계약) 구독의 대금 청구 소유권 이전](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [소유권 이전 FAQ](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [소유권 이전 문제 해결](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)