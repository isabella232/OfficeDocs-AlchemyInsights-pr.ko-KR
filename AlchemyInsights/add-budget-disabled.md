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
# <a name="why-is-the-add-budget-button-disabled-for-me"></a><span data-ttu-id="43d9b-102">예산 추가 단추가 비활성화된 이유는 무엇입니까?</span><span class="sxs-lookup"><span data-stu-id="43d9b-102">Why is the Add budget button disabled for me?</span></span>

<span data-ttu-id="43d9b-103">예산을 만들 수 있는 권한은 다음 중 하나에 해당합니다.</span><span class="sxs-lookup"><span data-stu-id="43d9b-103">To create a budget, you need one of the following permissions:</span></span>

- <span data-ttu-id="43d9b-104">관리 그룹, 구독, 리소스 그룹 범위</span><span class="sxs-lookup"><span data-stu-id="43d9b-104">Management Group, Subscription, Resource Group Scopes</span></span>
- <span data-ttu-id="43d9b-105">비용 관리 참가자</span><span class="sxs-lookup"><span data-stu-id="43d9b-105">Cost Management Contributor</span></span>
- <span data-ttu-id="43d9b-106">소유자</span><span class="sxs-lookup"><span data-stu-id="43d9b-106">Owner</span></span>
- <span data-ttu-id="43d9b-107">참가자</span><span class="sxs-lookup"><span data-stu-id="43d9b-107">Contributor</span></span>
- <span data-ttu-id="43d9b-108">엔터프라이즈 고객 전용: 등록, 부서, 계정 범위</span><span class="sxs-lookup"><span data-stu-id="43d9b-108">Enterprise Customer Only: Enrollment, Department, Account Scopes</span></span>
- <span data-ttu-id="43d9b-109">등록 관리자(등록 범위에서 예산 설정)</span><span class="sxs-lookup"><span data-stu-id="43d9b-109">Enrollment Admin (set budget at Enrollment scope)</span></span>
- <span data-ttu-id="43d9b-110">부서 관리자(부서 범위에서 예산 설정)</span><span class="sxs-lookup"><span data-stu-id="43d9b-110">Department Admin (set budget at Department scope)</span></span>
- <span data-ttu-id="43d9b-111">계정 소유자(계정 범위에서 예산 설정)</span><span class="sxs-lookup"><span data-stu-id="43d9b-111">Account Owner (set budget at Account scope)</span></span>
- <span data-ttu-id="43d9b-112">최신 고객 계약만: 청구 계정, 청구 프로필, 송장 섹션 범위</span><span class="sxs-lookup"><span data-stu-id="43d9b-112">Modern Customer Agreement Only: Billing Account, Billing Profile, Invoice Section Scopes</span></span>
- <span data-ttu-id="43d9b-113">Azure 구독 작성자</span><span class="sxs-lookup"><span data-stu-id="43d9b-113">Azure subscription creator</span></span>

<span data-ttu-id="43d9b-114">**현재 달의 비용이 이미 예산을 넘을 때 예산을 만들었다고 합니다. 경고가 수신되지 않은 이유는 무엇입니까?**</span><span class="sxs-lookup"><span data-stu-id="43d9b-114">**I created a budget when my cost for the current month was already over-budget. Why did I not receive an alert?**</span></span>  
<span data-ttu-id="43d9b-115">예산을 만들 때 이미 특정 비용 임계값을 초과한 경우 경고가 발생하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="43d9b-115">If you have already exceeded a given cost threshold when you create a budget that alert will not fire.</span></span> <span data-ttu-id="43d9b-116">새 주기가 시작되면 임계값을 위반하면 경고가 시작됩니다.</span><span class="sxs-lookup"><span data-stu-id="43d9b-116">Once a new cycle begins, if you breach the threshold then the alert will fire.</span></span>

<span data-ttu-id="43d9b-117">**정의된 예산 경고 임계값 중 하나를 초과한 후 경고를 수신할 것으로 예상되는 경우**</span><span class="sxs-lookup"><span data-stu-id="43d9b-117">**When should I expect to receive an alert after I exceed one of my defined budget alert thresholds?**</span></span>  
<span data-ttu-id="43d9b-118">예산은 4시간마다 평가됩니다.</span><span class="sxs-lookup"><span data-stu-id="43d9b-118">Budgets are evaluated every 4 hours.</span></span> <span data-ttu-id="43d9b-119">사용 현황 데이터가 예산 시스템에 도달하는 데 최소 8시간이 소요됩니다.</span><span class="sxs-lookup"><span data-stu-id="43d9b-119">It takes a minimum of 8 hours for usage data to reach the budgets system.</span></span> <span data-ttu-id="43d9b-120">이 경우 임계값을 초과한 후 경고가 발생하기까지 12시간 정도 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="43d9b-120">Given this, alerts may take as long as 12 hours to fire after you exceed a threshold.</span></span>

<span data-ttu-id="43d9b-121">**월 또는 청구 월 재설정 기간을 선택할 때 시작 날짜 단추를 사용하지 않도록 설정하는 이유는 무엇입니까?**</span><span class="sxs-lookup"><span data-stu-id="43d9b-121">**Why is the Start date button disabled when I select a Month or Billing month reset period?**</span></span>  
<span data-ttu-id="43d9b-122">예산은 현재 달 또는 현재 청구 기간에 맞춰 정렬됩니다(청구 월이 선택된 경우).</span><span class="sxs-lookup"><span data-stu-id="43d9b-122">Budgets are aligned to the current calendar month or current billing period (in the case where Billing Month is selected).</span></span> <span data-ttu-id="43d9b-123">따라서 이 값을 미리 채우면 됩니다.</span><span class="sxs-lookup"><span data-stu-id="43d9b-123">Therefore, we pre-populate this value for you.</span></span>

<span data-ttu-id="43d9b-124">**예산 생성 환경의 비용 그래프가 없는 이유는 무엇입니까?**</span><span class="sxs-lookup"><span data-stu-id="43d9b-124">**Why do I not see a graph of my costs in the budget creation experience?**</span></span>  
<span data-ttu-id="43d9b-125">예산 작성을 지원하기 위해 그래프를 렌더링하려면 최소 2개월의 비용 데이터가 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="43d9b-125">We need a minimum of 2 months of cost data before we can render a graph to assist you with budget creation.</span></span>

<span data-ttu-id="43d9b-126">**방금 만든 구독에 대해 예산을 설정할 수 없는 이유는 무엇입니까?**</span><span class="sxs-lookup"><span data-stu-id="43d9b-126">**Why can't I set a budget against a subscription I just created?**</span></span>  
<span data-ttu-id="43d9b-127">구독을 생성한 후 데이터를 처리하려면 24~48시간이 소요된 후 예산을 설정해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="43d9b-127">After the creation of a subscription, the data takes 24-48 hours to process before setting a budget against it.</span></span>

<span data-ttu-id="43d9b-128">**예산 API 리소스**</span><span class="sxs-lookup"><span data-stu-id="43d9b-128">**Budget API Resources**</span></span>

- <span data-ttu-id="43d9b-129">[Budgets API v1:](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support)예산을 만들고 업데이트하는 작업을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="43d9b-129">[Budgets API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): Provides operations to create and update budgets.</span></span> <span data-ttu-id="43d9b-130">예산 API를 사용하여 예산 임계값을 설정하고 해당 임계값에 도달할 때 실행하도록 여러 경고를 구성할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="43d9b-130">Using the Budgets API, you can set a budget threshold and configure multiple alerts to fire as you approach that threshold.</span></span> <span data-ttu-id="43d9b-131">알림은 자동화를 수행하기 위해 전자 메일 또는 Azure Action 그룹을 트리거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="43d9b-131">Alerts can trigger an email or an Azure Action Group to perform automation.</span></span> <span data-ttu-id="43d9b-132">참고: 이 API에 대한 필터링은 쿼리 API 필터링/차원과 일치하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="43d9b-132">Note: Filtering for this API does not align with Query API filtering / dimensions.</span></span>
- <span data-ttu-id="43d9b-133">[Budgets API v2:](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json)v1보다 높은 비용 필터링 기능을 사용하여 예산을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="43d9b-133">[Budgets API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): Create budgets with greater cost filtering capabilities than v1.</span></span> <span data-ttu-id="43d9b-134">필터링은 쿼리 및 차원 API에 사용되는 계약에 맞게 정렬됩니다.</span><span class="sxs-lookup"><span data-stu-id="43d9b-134">Filtering aligns to the contract used in our Query and Dimensions APIs.</span></span> <span data-ttu-id="43d9b-135">이 API는 앞으로 이동을 사용하는 데 권장되는 예산 API입니다.</span><span class="sxs-lookup"><span data-stu-id="43d9b-135">This is the recommended budgets API to use moving forward.</span></span>
- <span data-ttu-id="43d9b-136">[차원:](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support)다양한 범위에서 사용에 대해 지원되는 차원을 얻을 수 있는 작업을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="43d9b-136">[Dimensions](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): Provides operations to get supported dimensions for your usage under a variety of scopes.</span></span> <span data-ttu-id="43d9b-137">차원 API를 사용하여 쿼리 API를 사용하여 쿼리를 생성하기 위한 입력으로 사용할 수 있는 차원 목록을 검색할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="43d9b-137">Using the Dimensions API, you can retrieve a list of dimensions that can be used as inputs for generating queries with the Query API.</span></span>
- <span data-ttu-id="43d9b-138">[쿼리:](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support)제공하는 쿼리를 기반으로 집계 비용 및 사용 현황 데이터를 얻을 수 있는 작업을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="43d9b-138">[Query](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): Provides operations to get aggregated cost and usage data based on the query you supply.</span></span> <span data-ttu-id="43d9b-139">쿼리 API를 사용하여 사용 가능한 모든 차원(차원 API에서 액세스)에 대해 원하는 필터링, 정렬 및 그룹을 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="43d9b-139">Using the Query API, you can specify your desired filtering, sorting and grouping on all available dimensions (which are accessed from the Dimensions API).</span></span>

<span data-ttu-id="43d9b-140">**예상 비용**</span><span class="sxs-lookup"><span data-stu-id="43d9b-140">**Forecasted Costs**</span></span>

<span data-ttu-id="43d9b-141">**비용 분석에서 내 비용에 대한 예측이 없는 이유는 무엇입니까?**</span><span class="sxs-lookup"><span data-stu-id="43d9b-141">**Why don’t I see forecasts for my costs in Cost Analysis?**</span></span>  
<span data-ttu-id="43d9b-142">비용 분석에서 예측 예측이 누락될 수 있는 이유는 여러 가지가 있습니다. 그 중 일부는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="43d9b-142">There are multiple reasons why the forecast projection might be missing for you in Cost Analysis, some of them are as follows:</span></span>

1. <span data-ttu-id="43d9b-143">비용 데이터가 10일 미만이면 예측 차트가 로드되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="43d9b-143">If your cost data is less than 10 days old, the forecast chart will not load.</span></span> <span data-ttu-id="43d9b-144">정확한 예측을 위해 이 모델에는 최신 비용 데이터가 10일 이상 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="43d9b-144">The model requires at least 10 days of recent cost data for accurate projections</span></span>
2. <span data-ttu-id="43d9b-145">기록 날짜를 선택한 경우 예측 차트가 표시되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="43d9b-145">If you have selected historic dates, then the forecast chart will not be visible.</span></span> <span data-ttu-id="43d9b-146">예측 차트가 표시될 향후 날짜가 있는 날짜 범위를 선택하십시오.</span><span class="sxs-lookup"><span data-stu-id="43d9b-146">Please select a date range with future dates for the forecast chart to be displayed</span></span>
3. <span data-ttu-id="43d9b-147">계정에 통화가 여러 개 있는 경우 예측 차트는 '모든 비용(USD)'에 대한 프로젝트 비용만 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="43d9b-147">If your account has multiple currencies, the forecast chart will only project costs for 'All costs in USD'</span></span>

<span data-ttu-id="43d9b-148">**자원을 변경할 때 예측이 변경되지 않는 이유는 무엇입니까?**</span><span class="sxs-lookup"><span data-stu-id="43d9b-148">**Why doesn’t the forecast change when I make changes to my resources?**</span></span>  
<span data-ttu-id="43d9b-149">예측 모델에서는 계정 변경을 고려하기 위해 며칠이 필요하며 리소스 변경에 따라 즉각적인 예상을 수행하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="43d9b-149">The forecast model requires a couple of days to account for changes in the account and does not make immediate projections based on change in resources</span></span>  
<span data-ttu-id="43d9b-150">더 큰 리소스 증가 또는 감소 단계의 경우 이 변경 내용을 변호에 맞게 조정하는 데 모델이 약간 더 오래 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="43d9b-150">For larger steps of increase or decrease in resources, the model will take slightly longer to adjust to these changes to account for anomalies</span></span>

<span data-ttu-id="43d9b-151">**예약 또는 마켓플레이스 구매 후 예측이 증가하는 이유는 무엇입니까?**</span><span class="sxs-lookup"><span data-stu-id="43d9b-151">**Why does my forecast increase after I make a reservation or Marketplace purchase?**</span></span>  
<span data-ttu-id="43d9b-152">예측 모델은 '실제 비용'을 고려하며 사용량과 구매를 별도로 고려하지 않습니다. 일회성 구매의 경우 이 모델은 갑작스러운 비용 증가를 고려하여 10일 후의 투영을 줄입니다.</span><span class="sxs-lookup"><span data-stu-id="43d9b-152">The forecast model considers your 'Actual Cost' and does not account for usage and purchase separately.For a one-time purchase, the model will decrease the projections after 10 days to account for the sudden increase in costs</span></span>

<span data-ttu-id="43d9b-153">**단일 차원에 대한 예측(예: Meter)**</span><span class="sxs-lookup"><span data-stu-id="43d9b-153">**I want to see forecasts for a single dimension (eg. Meter)**</span></span>  
<span data-ttu-id="43d9b-154">Forecast는 현재 개별 미터가 아닌 총 비용 투영을 지원하고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="43d9b-154">Forecast currently supports total cost projections and not for individual meters.</span></span> <span data-ttu-id="43d9b-155">따라서 '차원으로 그룹화'를 할 때 차원의 모든 항목의 합계에 대한 투영이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="43d9b-155">Hence, when 'Grouped by' a dimension, the projections will be for total of all items in the dimension</span></span>

<span data-ttu-id="43d9b-156">**권장 문서**</span><span class="sxs-lookup"><span data-stu-id="43d9b-156">**Recommended Documents**</span></span>

- [<span data-ttu-id="43d9b-157">Azure 비용 관리란?</span><span class="sxs-lookup"><span data-stu-id="43d9b-157">What is Azure Cost Management?</span></span>](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="43d9b-158">Azure 비용 관리 모범 사례</span><span class="sxs-lookup"><span data-stu-id="43d9b-158">Azure Cost Management best practices</span></span>](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="43d9b-159">비용 및 지출 분석</span><span class="sxs-lookup"><span data-stu-id="43d9b-159">Analyze your costs and spending</span></span>](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="43d9b-160">비용 분석을 사용하여 비용 탐색 및 분석</span><span class="sxs-lookup"><span data-stu-id="43d9b-160">Explore and analyze costs with Cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="43d9b-161">Azure 비용 관리: 가격 책정</span><span class="sxs-lookup"><span data-stu-id="43d9b-161">Azure Cost Management: Pricing</span></span>](https://azure.microsoft.com/services/cost-management/#pricing)
- [<span data-ttu-id="43d9b-162">비용 분석의 비용 검토</span><span class="sxs-lookup"><span data-stu-id="43d9b-162">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [<span data-ttu-id="43d9b-163">비디오 자습서: Azure Portal에서 예산 만들기</span><span class="sxs-lookup"><span data-stu-id="43d9b-163">Video tutorial: Create a budget in the Azure portal</span></span>](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [<span data-ttu-id="43d9b-164">예산 보기 및 사용자 지정을 위한 선행 준비</span><span class="sxs-lookup"><span data-stu-id="43d9b-164">Prerequisites for viewing and customizing budgets</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [<span data-ttu-id="43d9b-165">예산 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="43d9b-165">Create and manage budgets</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [<span data-ttu-id="43d9b-166">Azure Action Groups 및 Budgets API를 사용하여 자동화 구성</span><span class="sxs-lookup"><span data-stu-id="43d9b-166">Configure automation with Azure Action Groups and Budgets API</span></span>](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [<span data-ttu-id="43d9b-167">비용 알림을 사용하여 사용량 및 지출 모니터링</span><span class="sxs-lookup"><span data-stu-id="43d9b-167">Use cost alerts to monitor usage and spending</span></span>](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="43d9b-168">비용 관리 모범 사례</span><span class="sxs-lookup"><span data-stu-id="43d9b-168">Cost Management best practices</span></span>](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

<span data-ttu-id="43d9b-169">**자습서 비디오**</span><span class="sxs-lookup"><span data-stu-id="43d9b-169">**Tutorial videos**</span></span>

- [<span data-ttu-id="43d9b-170">Azure Portal에서 예산 만들기</span><span class="sxs-lookup"><span data-stu-id="43d9b-170">Create a budget in the Azure portal</span></span>](https://go.microsoft.com/fwlink/?linkid=2146761)
- [<span data-ttu-id="43d9b-171">예산 API 및 작업 그룹을 사용하여 비용 관리</span><span class="sxs-lookup"><span data-stu-id="43d9b-171">Manage costs with the Budgets API and Action Groups</span></span>](https://go.microsoft.com/fwlink/?linkid=2147038)