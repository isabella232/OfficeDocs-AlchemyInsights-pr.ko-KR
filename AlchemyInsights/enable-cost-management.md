---
title: 비용 관리 사용
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 62f3cfb161c4f8da735bd288a2d6e22971b4aada
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325469"
---
# <a name="enable-cost-management"></a>비용 관리 사용

**'조직에 대해 비용이 사용하지 않도록 설정되어 있습니다'는 무엇을 의미하나요?**

EA(기업계약) 또는 MCA(Microsoft 고객 계약) 계정을 사용하는 조직은 비용 정보 및 가격 정보에 대한 액세스를 사용하지 않도록 설정할 수 있습니다.

Azure Portal에 로그인한 후 청구 API를 사용하여 프로그래밍식으로 송장(옵트인된 경우) 및 사용 현황 세부 정보를 받을 수 있습니다.

**추가 사용자가 송장에 액세스할 수 있도록 허용하는 방법**

1. Azure **Portal에서 구독** 블레이드로 이동하세요.
2. 송장을 **선택한** 다음 **송장에 액세스 를 선택합니다.**
3. 구독 범위 역할의 사용자가 송장을 다운로드할 수 있도록 액세스를 켜고 변경 내용을 저장합니다.

**참고:** 계정 관리자는 전자 메일을 통해 송장을 보내도록 구성할 수도 있습니다. 자세한 내용은 전자 [메일로 송장 보기를 참조하세요.](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?)

**청구 독자 역할에 사용자를 추가하는 방법**

1. Azure **Portal에서 구독** 블레이드로 이동하세요.
2. **IAM(액세스 제어)을 선택하고** 추가를 **클릭합니다.**
3. 역할 선택 페이지에서 청구 **독자를** 선택합니다. 
4. 초대할 사용자의 전자 메일을 입력한 다음 **확인을** 클릭하여 초대를 전송합니다.
5. 초대 전자 메일에 제공된 지침에 따라 청구 독자로 로그인합니다. 자세한 내용은 [청구에 대한 액세스 권한 부여를 참조하세요.](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in)

**추천 문서**

- [EA 포털을 통해 DA 및 AO 보기 사용](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [비용 관리에 포함된 비용](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [지원되는 Microsoft Azure 제공](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [비용 분석의 비용 검토](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [청구 정보에 대한 액세스 제공](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Microsoft 고객 계약에 대한 액세스 확인](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






