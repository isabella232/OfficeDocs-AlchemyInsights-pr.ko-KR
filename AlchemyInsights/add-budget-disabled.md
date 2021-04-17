---
title: 예산 추가 단추가 비활성화된 이유는 무엇입니까?
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
- "9003547"
- "6464"
ms.openlocfilehash: 426a54ea22490dcc47f40fd990654b2cf051a058
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822641"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>예산 추가 단추가 비활성화된 이유는 무엇입니까?

예산을 만들 수 있는 권한은 다음 중 하나에 해당합니다.

- 관리 그룹, 구독, 리소스 그룹 범위
- 비용 관리 참가자
- 소유자
- 참가자
- 엔터프라이즈 고객 전용: 등록, 부서, 계정 범위
- 등록 관리자(등록 범위에서 예산 설정)
- 부서 관리자(부서 범위에서 예산 설정)
- 계정 소유자(계정 범위에서 예산 설정)
- 최신 고객 계약만: 청구 계정, 청구 프로필, 송장 섹션 범위
- Azure 구독 작성자

**현재 달의 비용이 이미 예산을 넘을 때 예산을 만들었다고 합니다. 경고가 수신되지 않은 이유는 무엇입니까?**  
예산을 만들 때 이미 특정 비용 임계값을 초과한 경우 경고가 발생하지 않습니다. 새 주기가 시작되면 임계값을 위반하면 경고가 시작됩니다.

**정의된 예산 경고 임계값 중 하나를 초과한 후 경고를 수신할 것으로 예상되는 경우**  
예산은 4시간마다 평가됩니다. 사용 현황 데이터가 예산 시스템에 도달하는 데 최소 8시간이 소요됩니다. 이 경우 임계값을 초과한 후 경고가 발생하기까지 12시간 정도 걸릴 수 있습니다.

**월 또는 청구 월 재설정 기간을 선택할 때 시작 날짜 단추를 사용하지 않도록 설정하는 이유는 무엇입니까?**  
예산은 현재 달 또는 현재 청구 기간에 맞춰 정렬됩니다(청구 월이 선택된 경우). 따라서 이 값을 미리 채우면 됩니다.

**예산 생성 환경의 비용 그래프가 없는 이유는 무엇입니까?**  
예산 작성을 지원하기 위해 그래프를 렌더링하려면 최소 2개월의 비용 데이터가 필요합니다.

**방금 만든 구독에 대해 예산을 설정할 수 없는 이유는 무엇입니까?**  
구독을 생성한 후 데이터를 처리하려면 24~48시간이 소요된 후 예산을 설정해야 합니다.

**예산 API 리소스**

- [Budgets API v1:](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support)예산을 만들고 업데이트하는 작업을 제공합니다. 예산 API를 사용하여 예산 임계값을 설정하고 해당 임계값에 도달할 때 실행하도록 여러 경고를 구성할 수 있습니다. 알림은 자동화를 수행하기 위해 전자 메일 또는 Azure Action 그룹을 트리거할 수 있습니다. 참고: 이 API에 대한 필터링은 쿼리 API 필터링/차원과 일치하지 않습니다.
- [Budgets API v2:](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json)v1보다 높은 비용 필터링 기능을 사용하여 예산을 만들 수 있습니다. 필터링은 쿼리 및 차원 API에 사용되는 계약에 맞게 정렬됩니다. 이 API는 앞으로 이동을 사용하는 데 권장되는 예산 API입니다.
- [차원:](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support)다양한 범위에서 사용에 대해 지원되는 차원을 얻을 수 있는 작업을 제공합니다. 차원 API를 사용하여 쿼리 API를 사용하여 쿼리를 생성하기 위한 입력으로 사용할 수 있는 차원 목록을 검색할 수 있습니다.
- [쿼리:](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support)제공하는 쿼리를 기반으로 집계 비용 및 사용 현황 데이터를 얻을 수 있는 작업을 제공합니다. 쿼리 API를 사용하여 사용 가능한 모든 차원(차원 API에서 액세스)에 대해 원하는 필터링, 정렬 및 그룹을 지정할 수 있습니다.

**예상 비용**

**비용 분석에서 내 비용에 대한 예측이 없는 이유는 무엇입니까?**  
비용 분석에서 예측 예측이 누락될 수 있는 이유는 여러 가지가 있습니다. 그 중 일부는 다음과 같습니다.

1. 비용 데이터가 10일 미만이면 예측 차트가 로드되지 않습니다. 정확한 예측을 위해 이 모델에는 최신 비용 데이터가 10일 이상 필요합니다.
2. 기록 날짜를 선택한 경우 예측 차트가 표시되지 않습니다. 예측 차트가 표시될 향후 날짜가 있는 날짜 범위를 선택하십시오.
3. 계정에 통화가 여러 개 있는 경우 예측 차트는 '모든 비용(USD)'에 대한 프로젝트 비용만 제공합니다.

**자원을 변경할 때 예측이 변경되지 않는 이유는 무엇입니까?**  
예측 모델에서는 계정 변경을 고려하기 위해 며칠이 필요하며 리소스 변경에 따라 즉각적인 예상을 수행하지 않습니다.  
더 큰 리소스 증가 또는 감소 단계의 경우 이 변경 내용을 변호에 맞게 조정하는 데 모델이 약간 더 오래 걸릴 수 있습니다.

**예약 또는 마켓플레이스 구매 후 예측이 증가하는 이유는 무엇입니까?**  
예측 모델은 '실제 비용'을 고려하며 사용량과 구매를 별도로 고려하지 않습니다. 일회성 구매의 경우 이 모델은 갑작스러운 비용 증가를 고려하여 10일 후의 투영을 줄입니다.

**단일 차원에 대한 예측(예: Meter)**  
Forecast는 현재 개별 미터가 아닌 총 비용 투영을 지원하고 있습니다. 따라서 '차원으로 그룹화'를 할 때 차원의 모든 항목의 합계에 대한 투영이 됩니다.

**권장 문서**

- [Azure 비용 관리란?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure 비용 관리 모범 사례](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [비용 및 지출 분석](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [비용 분석을 사용하여 비용 탐색 및 분석](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure 비용 관리: 가격 책정](https://azure.microsoft.com/services/cost-management/#pricing)
- [비용 분석의 비용 검토](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [비디오 자습서: Azure Portal에서 예산 만들기](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [예산 보기 및 사용자 지정을 위한 선행 준비](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [예산 만들기 및 관리](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Azure Action Groups 및 Budgets API를 사용하여 자동화 구성](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [비용 알림을 사용하여 사용량 및 지출 모니터링](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [비용 관리 모범 사례](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**자습서 비디오**

- [Azure Portal에서 예산 만들기](https://go.microsoft.com/fwlink/?linkid=2146761)
- [예산 API 및 작업 그룹을 사용하여 비용 관리](https://go.microsoft.com/fwlink/?linkid=2147038)