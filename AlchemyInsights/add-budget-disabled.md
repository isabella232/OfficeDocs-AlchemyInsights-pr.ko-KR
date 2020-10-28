---
title: 지출 추가 단추를 사용할 수 없는 이유는 무엇 인가요?
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
- "9003547"
- "6464"
ms.openlocfilehash: 18edad73f617ba180cb08576ee6e5fa8faf07128
ms.sourcegitcommit: 9a7b85eae0bb775bc2498a83d8f5fedb72a6451e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/27/2020
ms.locfileid: "48769591"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>지출 추가 단추를 사용할 수 없는 이유는 무엇 인가요?

예산을 만들려면 다음 권한 중 하나가 필요 합니다.

- 관리 그룹, 구독, 리소스 그룹 범위
- 비용 관리 참가자
- 소유자
- 참가자
- Enterprise 고객만: 등록, 부서, 계정 범위
- 등록 관리자 (등록 범위의 예산 설정)
- 부서 관리자 (부서 범위의 예산 설정)
- 계정 소유자 (계정 범위의 예산 설정)
- 최신 고객 계약 전용: 청구 계정, 청구 프로필, 송장 섹션 범위
- Azure 구독 작성자

**이번 달의 비용이 이미 예산에 도달 했을 때 예산을 만들었습니다. 경고가 표시 되지 않는 이유는 무엇 인가요?**  
경고가 발생 하지 않는 예산을 만들 때 이미 지정 된 비용 임계값을 초과 하는 경우 새 주기가 시작 되 고 임계값을 위반 하면 경고가 발생 합니다.

**정의 된 예산 경고 임계값 중 하나를 초과 하면 경고가 수신 될 것으로 예상 되는 시기**  
예산은 4 시간 마다 평가 됩니다. 사용 현황 데이터가 예산 시스템에 도달 하는 데 최소 8 시간이 소요 됩니다. 이 경우 임계값을 초과 하면 경고를 발생 시키기 위해 12 시간까지 걸릴 수 있습니다.

**월 또는 대금 청구 월 재설정 기간을 선택할 때 시작 날짜 단추를 사용할 수 없는 이유는 무엇입니까?**  
예산이 현재 달 또는 현재 대금 청구 기간 (대금 청구 월이 선택 된 경우)에 정렬 됩니다. 따라서이 값을 미리 채웁니다.

**예산 제작 환경에서 내 비용 그래프가 표시 되지 않는 이유는 무엇 인가요?**  
예산 생성을 지원 하기 위해 그래프를 렌더링 하려면 최소한 2 개월의 비용 데이터가 필요 합니다.

**방금 만든 구독에 대해 예산을 설정할 수 없는 이유는 무엇 인가요?**  
구독을 만든 후에는 데이터에 대해 예산을 설정 하기 전에 처리 하는 데 24-48 시간이 소요 됩니다.

**예산 API 리소스**

- [예산 API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): 예산 만들기 및 업데이트 작업을 제공 합니다. 예산 API를 사용 하 여 예산의 임계값을 설정 하 고이 임계값에 근접 하면 여러 경고를 구성할 수 있습니다. 경고는 전자 메일 또는 Azure 작업 그룹을 트리거하여 자동화를 수행할 수 있습니다. 참고:이 API에 대 한 필터링은 쿼리 API 필터링/차원에 맞지 않습니다.
- [예산 API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): v1 보다 더 큰 비용 필터링 기능을 사용 하 여 예산을 만듭니다. 필터링은 쿼리 및 차원 Api에 사용 된 계약에 맞게 정렬 됩니다. 앞으로 이동 하는 데 권장 되는 예산 API입니다.
- [차원](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): 다양 한 범위의 사용에 대해 지원 되는 차원을 가져오는 작업을 제공 합니다. 차원 API를 사용 하 여 쿼리 API를 사용 하 여 쿼리 생성을 위한 입력으로 사용할 수 있는 차원 목록을 검색할 수 있습니다.
- [쿼리](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): 제공한 쿼리에 따라 집계 된 비용 및 사용 현황 데이터를 가져오는 작업을 제공 합니다. 쿼리 API를 사용 하 여 사용 가능한 모든 차원 (차원 API에서 액세스)에 원하는 필터링, 정렬 및 그룹화를 지정할 수 있습니다.

**예상 비용**

**비용 분석의 비용에 대 한 예측을 확인할 이유가 없는 이유는 무엇 인가요?**  
비용 분석에서 예측 프로젝션이 누락 될 수 있는 몇 가지 이유는 다음과 같습니다.

1. 비용 데이터가 10 일 보다 작으면 예측 차트가 로드 되지 않습니다. 모델을 정확 하 게 프로젝션 하려면 최근 비용 데이터가 10 일 이상 필요 합니다.
2. 날짜 기록을 선택 하면 예측 차트가 표시 되지 않습니다. 예측 차트를 표시할 날짜 범위를 미래 날짜로 선택 하세요.
3. 사용자의 계정에 통화가 여러 개 있는 경우 예측 차트에는 ' 모든 비용이 USD 인 '의 비용만 프로젝트 비용이 듭니다.

**자원을 변경할 때 예측이 변경 되지 않는 이유는 무엇 인가요?**  
예측 모델에서 계정의 변경 내용을 고려 하 고 리소스 변경에 따라 즉각적인 예측을 수행 하지 않으려면 몇 일이 소요 됩니다.  
리소스의 증가 또는 감소에 대 한 보다 큰 단계를 수행 하는 경우에는 예외를 고려 하 여 이러한 변경 사항에 맞게 조정 하는 데 더 오래 걸립니다.

**예약 또는 마켓플레이스 구매를 수행한 후에도 예측이 향상 되는 이유는 무엇 인가요?**  
예측 모델에서는 ' 실제 비용 '을 고려 하며 사용 현황 및 구매를 별도로 고려 하지 않습니다. 일회성 구매의 경우 모델이 갑작스런 비용 증가를 고려 하 여 10 일 후의 예측을 감소 시킵니다.

**단일 차원에 대 한 예측을 보려는 경우 (예를 들어, 1m**  
예측은 현재 개별 측정기가 아닌 총 비용 프로젝션을 지원 합니다. 따라서 ' 그룹화 '로 지정한 경우에는 차원의 모든 항목에 대 한 합계를 예측 하 게 됩니다.

**권장 문서**

- [Azure 비용 관리 란?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure 비용 관리 모범 사례](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [비용 및 지출 분석](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [비용 분석을 사용한 비용 탐색 및 분석](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure 비용 관리: 가격 책정](https://azure.microsoft.com/services/cost-management/#pricing)
- [비용 분석의 비용 검토](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [비디오 자습서: Azure 포털에 예산 만들기](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [예산 보기 및 사용자 지정을 위한 필수 구성 요소](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [예산 만들기 및 관리](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Azure 작업 그룹 및 예산 API를 사용 하 여 자동화 구성](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [비용 알림을 사용 하 여 사용 현황 및 비용 모니터링](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [비용 관리 모범 사례](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**자습서 동영상**

- [Azure 포털에서 예산 만들기](https://go.microsoft.com/fwlink/?linkid=2146761)
- [예산 API 및 작업 그룹을 사용한 비용 관리](https://go.microsoft.com/fwlink/?linkid=2147038)