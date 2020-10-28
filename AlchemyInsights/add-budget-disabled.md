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
# <a name="why-is-the-add-budget-button-disabled-for-me"></a><span data-ttu-id="8cd18-102">지출 추가 단추를 사용할 수 없는 이유는 무엇 인가요?</span><span class="sxs-lookup"><span data-stu-id="8cd18-102">Why is the Add budget button disabled for me?</span></span>

<span data-ttu-id="8cd18-103">예산을 만들려면 다음 권한 중 하나가 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="8cd18-103">To create a budget, you need one of the following permissions:</span></span>

- <span data-ttu-id="8cd18-104">관리 그룹, 구독, 리소스 그룹 범위</span><span class="sxs-lookup"><span data-stu-id="8cd18-104">Management Group, Subscription, Resource Group Scopes</span></span>
- <span data-ttu-id="8cd18-105">비용 관리 참가자</span><span class="sxs-lookup"><span data-stu-id="8cd18-105">Cost Management Contributor</span></span>
- <span data-ttu-id="8cd18-106">소유자</span><span class="sxs-lookup"><span data-stu-id="8cd18-106">Owner</span></span>
- <span data-ttu-id="8cd18-107">참가자</span><span class="sxs-lookup"><span data-stu-id="8cd18-107">Contributor</span></span>
- <span data-ttu-id="8cd18-108">Enterprise 고객만: 등록, 부서, 계정 범위</span><span class="sxs-lookup"><span data-stu-id="8cd18-108">Enterprise Customer Only: Enrollment, Department, Account Scopes</span></span>
- <span data-ttu-id="8cd18-109">등록 관리자 (등록 범위의 예산 설정)</span><span class="sxs-lookup"><span data-stu-id="8cd18-109">Enrollment Admin (set budget at Enrollment scope)</span></span>
- <span data-ttu-id="8cd18-110">부서 관리자 (부서 범위의 예산 설정)</span><span class="sxs-lookup"><span data-stu-id="8cd18-110">Department Admin (set budget at Department scope)</span></span>
- <span data-ttu-id="8cd18-111">계정 소유자 (계정 범위의 예산 설정)</span><span class="sxs-lookup"><span data-stu-id="8cd18-111">Account Owner (set budget at Account scope)</span></span>
- <span data-ttu-id="8cd18-112">최신 고객 계약 전용: 청구 계정, 청구 프로필, 송장 섹션 범위</span><span class="sxs-lookup"><span data-stu-id="8cd18-112">Modern Customer Agreement Only: Billing Account, Billing Profile, Invoice Section Scopes</span></span>
- <span data-ttu-id="8cd18-113">Azure 구독 작성자</span><span class="sxs-lookup"><span data-stu-id="8cd18-113">Azure subscription creator</span></span>

<span data-ttu-id="8cd18-114">**이번 달의 비용이 이미 예산에 도달 했을 때 예산을 만들었습니다. 경고가 표시 되지 않는 이유는 무엇 인가요?**</span><span class="sxs-lookup"><span data-stu-id="8cd18-114">**I created a budget when my cost for the current month was already over-budget. Why did I not receive an alert?**</span></span>  
<span data-ttu-id="8cd18-115">경고가 발생 하지 않는 예산을 만들 때 이미 지정 된 비용 임계값을 초과 하는 경우</span><span class="sxs-lookup"><span data-stu-id="8cd18-115">If you have already exceeded a given cost threshold when you create a budget that alert will not fire.</span></span> <span data-ttu-id="8cd18-116">새 주기가 시작 되 고 임계값을 위반 하면 경고가 발생 합니다.</span><span class="sxs-lookup"><span data-stu-id="8cd18-116">Once a new cycle begins, if you breach the threshold then the alert will fire.</span></span>

<span data-ttu-id="8cd18-117">**정의 된 예산 경고 임계값 중 하나를 초과 하면 경고가 수신 될 것으로 예상 되는 시기**</span><span class="sxs-lookup"><span data-stu-id="8cd18-117">**When should I expect to receive an alert after I exceed one of my defined budget alert thresholds?**</span></span>  
<span data-ttu-id="8cd18-118">예산은 4 시간 마다 평가 됩니다.</span><span class="sxs-lookup"><span data-stu-id="8cd18-118">Budgets are evaluated every 4 hours.</span></span> <span data-ttu-id="8cd18-119">사용 현황 데이터가 예산 시스템에 도달 하는 데 최소 8 시간이 소요 됩니다.</span><span class="sxs-lookup"><span data-stu-id="8cd18-119">It takes a minimum of 8 hours for usage data to reach the budgets system.</span></span> <span data-ttu-id="8cd18-120">이 경우 임계값을 초과 하면 경고를 발생 시키기 위해 12 시간까지 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8cd18-120">Given this, alerts may take as long as 12 hours to fire after you exceed a threshold.</span></span>

<span data-ttu-id="8cd18-121">**월 또는 대금 청구 월 재설정 기간을 선택할 때 시작 날짜 단추를 사용할 수 없는 이유는 무엇입니까?**</span><span class="sxs-lookup"><span data-stu-id="8cd18-121">**Why is the Start date button disabled when I select a Month or Billing month reset period?**</span></span>  
<span data-ttu-id="8cd18-122">예산이 현재 달 또는 현재 대금 청구 기간 (대금 청구 월이 선택 된 경우)에 정렬 됩니다.</span><span class="sxs-lookup"><span data-stu-id="8cd18-122">Budgets are aligned to the current calendar month or current billing period (in the case where Billing Month is selected).</span></span> <span data-ttu-id="8cd18-123">따라서이 값을 미리 채웁니다.</span><span class="sxs-lookup"><span data-stu-id="8cd18-123">Therefore, we pre-populate this value for you.</span></span>

<span data-ttu-id="8cd18-124">**예산 제작 환경에서 내 비용 그래프가 표시 되지 않는 이유는 무엇 인가요?**</span><span class="sxs-lookup"><span data-stu-id="8cd18-124">**Why do I not see a graph of my costs in the budget creation experience?**</span></span>  
<span data-ttu-id="8cd18-125">예산 생성을 지원 하기 위해 그래프를 렌더링 하려면 최소한 2 개월의 비용 데이터가 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="8cd18-125">We need a minimum of 2 months of cost data before we can render a graph to assist you with budget creation.</span></span>

<span data-ttu-id="8cd18-126">**방금 만든 구독에 대해 예산을 설정할 수 없는 이유는 무엇 인가요?**</span><span class="sxs-lookup"><span data-stu-id="8cd18-126">**Why can't I set a budget against a subscription I just created?**</span></span>  
<span data-ttu-id="8cd18-127">구독을 만든 후에는 데이터에 대해 예산을 설정 하기 전에 처리 하는 데 24-48 시간이 소요 됩니다.</span><span class="sxs-lookup"><span data-stu-id="8cd18-127">After the creation of a subscription, the data takes 24-48 hours to process before setting a budget against it.</span></span>

<span data-ttu-id="8cd18-128">**예산 API 리소스**</span><span class="sxs-lookup"><span data-stu-id="8cd18-128">**Budget API Resources**</span></span>

- <span data-ttu-id="8cd18-129">[예산 API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): 예산 만들기 및 업데이트 작업을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="8cd18-129">[Budgets API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): Provides operations to create and update budgets.</span></span> <span data-ttu-id="8cd18-130">예산 API를 사용 하 여 예산의 임계값을 설정 하 고이 임계값에 근접 하면 여러 경고를 구성할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8cd18-130">Using the Budgets API, you can set a budget threshold and configure multiple alerts to fire as you approach that threshold.</span></span> <span data-ttu-id="8cd18-131">경고는 전자 메일 또는 Azure 작업 그룹을 트리거하여 자동화를 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8cd18-131">Alerts can trigger an email or an Azure Action Group to perform automation.</span></span> <span data-ttu-id="8cd18-132">참고:이 API에 대 한 필터링은 쿼리 API 필터링/차원에 맞지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="8cd18-132">Note: Filtering for this API does not align with Query API filtering / dimensions.</span></span>
- <span data-ttu-id="8cd18-133">[예산 API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): v1 보다 더 큰 비용 필터링 기능을 사용 하 여 예산을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="8cd18-133">[Budgets API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): Create budgets with greater cost filtering capabilities than v1.</span></span> <span data-ttu-id="8cd18-134">필터링은 쿼리 및 차원 Api에 사용 된 계약에 맞게 정렬 됩니다.</span><span class="sxs-lookup"><span data-stu-id="8cd18-134">Filtering aligns to the contract used in our Query and Dimensions APIs.</span></span> <span data-ttu-id="8cd18-135">앞으로 이동 하는 데 권장 되는 예산 API입니다.</span><span class="sxs-lookup"><span data-stu-id="8cd18-135">This is the recommended budgets API to use moving forward.</span></span>
- <span data-ttu-id="8cd18-136">[차원](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): 다양 한 범위의 사용에 대해 지원 되는 차원을 가져오는 작업을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="8cd18-136">[Dimensions](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): Provides operations to get supported dimensions for your usage under a variety of scopes.</span></span> <span data-ttu-id="8cd18-137">차원 API를 사용 하 여 쿼리 API를 사용 하 여 쿼리 생성을 위한 입력으로 사용할 수 있는 차원 목록을 검색할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8cd18-137">Using the Dimensions API, you can retrieve a list of dimensions that can be used as inputs for generating queries with the Query API.</span></span>
- <span data-ttu-id="8cd18-138">[쿼리](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): 제공한 쿼리에 따라 집계 된 비용 및 사용 현황 데이터를 가져오는 작업을 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="8cd18-138">[Query](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): Provides operations to get aggregated cost and usage data based on the query you supply.</span></span> <span data-ttu-id="8cd18-139">쿼리 API를 사용 하 여 사용 가능한 모든 차원 (차원 API에서 액세스)에 원하는 필터링, 정렬 및 그룹화를 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8cd18-139">Using the Query API, you can specify your desired filtering, sorting and grouping on all available dimensions (which are accessed from the Dimensions API).</span></span>

<span data-ttu-id="8cd18-140">**예상 비용**</span><span class="sxs-lookup"><span data-stu-id="8cd18-140">**Forecasted Costs**</span></span>

<span data-ttu-id="8cd18-141">**비용 분석의 비용에 대 한 예측을 확인할 이유가 없는 이유는 무엇 인가요?**</span><span class="sxs-lookup"><span data-stu-id="8cd18-141">**Why don’t I see forecasts for my costs in Cost Analysis?**</span></span>  
<span data-ttu-id="8cd18-142">비용 분석에서 예측 프로젝션이 누락 될 수 있는 몇 가지 이유는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="8cd18-142">There are multiple reasons why the forecast projection might be missing for you in Cost Analysis, some of them are as follows:</span></span>

1. <span data-ttu-id="8cd18-143">비용 데이터가 10 일 보다 작으면 예측 차트가 로드 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="8cd18-143">If your cost data is less than 10 days old, the forecast chart will not load.</span></span> <span data-ttu-id="8cd18-144">모델을 정확 하 게 프로젝션 하려면 최근 비용 데이터가 10 일 이상 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="8cd18-144">The model requires at least 10 days of recent cost data for accurate projections</span></span>
2. <span data-ttu-id="8cd18-145">날짜 기록을 선택 하면 예측 차트가 표시 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="8cd18-145">If you have selected historic dates, then the forecast chart will not be visible.</span></span> <span data-ttu-id="8cd18-146">예측 차트를 표시할 날짜 범위를 미래 날짜로 선택 하세요.</span><span class="sxs-lookup"><span data-stu-id="8cd18-146">Please select a date range with future dates for the forecast chart to be displayed</span></span>
3. <span data-ttu-id="8cd18-147">사용자의 계정에 통화가 여러 개 있는 경우 예측 차트에는 ' 모든 비용이 USD 인 '의 비용만 프로젝트 비용이 듭니다.</span><span class="sxs-lookup"><span data-stu-id="8cd18-147">If your account has multiple currencies, the forecast chart will only project costs for 'All costs in USD'</span></span>

<span data-ttu-id="8cd18-148">**자원을 변경할 때 예측이 변경 되지 않는 이유는 무엇 인가요?**</span><span class="sxs-lookup"><span data-stu-id="8cd18-148">**Why doesn’t the forecast change when I make changes to my resources?**</span></span>  
<span data-ttu-id="8cd18-149">예측 모델에서 계정의 변경 내용을 고려 하 고 리소스 변경에 따라 즉각적인 예측을 수행 하지 않으려면 몇 일이 소요 됩니다.</span><span class="sxs-lookup"><span data-stu-id="8cd18-149">The forecast model requires a couple of days to account for changes in the account and does not make immediate projections based on change in resources</span></span>  
<span data-ttu-id="8cd18-150">리소스의 증가 또는 감소에 대 한 보다 큰 단계를 수행 하는 경우에는 예외를 고려 하 여 이러한 변경 사항에 맞게 조정 하는 데 더 오래 걸립니다.</span><span class="sxs-lookup"><span data-stu-id="8cd18-150">For larger steps of increase or decrease in resources, the model will take slightly longer to adjust to these changes to account for anomalies</span></span>

<span data-ttu-id="8cd18-151">**예약 또는 마켓플레이스 구매를 수행한 후에도 예측이 향상 되는 이유는 무엇 인가요?**</span><span class="sxs-lookup"><span data-stu-id="8cd18-151">**Why does my forecast increase after I make a reservation or Marketplace purchase?**</span></span>  
<span data-ttu-id="8cd18-152">예측 모델에서는 ' 실제 비용 '을 고려 하며 사용 현황 및 구매를 별도로 고려 하지 않습니다. 일회성 구매의 경우 모델이 갑작스런 비용 증가를 고려 하 여 10 일 후의 예측을 감소 시킵니다.</span><span class="sxs-lookup"><span data-stu-id="8cd18-152">The forecast model considers your 'Actual Cost' and does not account for usage and purchase separately.For a one-time purchase, the model will decrease the projections after 10 days to account for the sudden increase in costs</span></span>

<span data-ttu-id="8cd18-153">**단일 차원에 대 한 예측을 보려는 경우 (예를 들어, 1m**</span><span class="sxs-lookup"><span data-stu-id="8cd18-153">**I want to see forecasts for a single dimension (eg. Meter)**</span></span>  
<span data-ttu-id="8cd18-154">예측은 현재 개별 측정기가 아닌 총 비용 프로젝션을 지원 합니다.</span><span class="sxs-lookup"><span data-stu-id="8cd18-154">Forecast currently supports total cost projections and not for individual meters.</span></span> <span data-ttu-id="8cd18-155">따라서 ' 그룹화 '로 지정한 경우에는 차원의 모든 항목에 대 한 합계를 예측 하 게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="8cd18-155">Hence, when 'Grouped by' a dimension, the projections will be for total of all items in the dimension</span></span>

<span data-ttu-id="8cd18-156">**권장 문서**</span><span class="sxs-lookup"><span data-stu-id="8cd18-156">**Recommended Documents**</span></span>

- [<span data-ttu-id="8cd18-157">Azure 비용 관리 란?</span><span class="sxs-lookup"><span data-stu-id="8cd18-157">What is Azure Cost Management?</span></span>](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="8cd18-158">Azure 비용 관리 모범 사례</span><span class="sxs-lookup"><span data-stu-id="8cd18-158">Azure Cost Management best practices</span></span>](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="8cd18-159">비용 및 지출 분석</span><span class="sxs-lookup"><span data-stu-id="8cd18-159">Analyze your costs and spending</span></span>](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="8cd18-160">비용 분석을 사용한 비용 탐색 및 분석</span><span class="sxs-lookup"><span data-stu-id="8cd18-160">Explore and analyze costs with Cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="8cd18-161">Azure 비용 관리: 가격 책정</span><span class="sxs-lookup"><span data-stu-id="8cd18-161">Azure Cost Management: Pricing</span></span>](https://azure.microsoft.com/services/cost-management/#pricing)
- [<span data-ttu-id="8cd18-162">비용 분석의 비용 검토</span><span class="sxs-lookup"><span data-stu-id="8cd18-162">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [<span data-ttu-id="8cd18-163">비디오 자습서: Azure 포털에 예산 만들기</span><span class="sxs-lookup"><span data-stu-id="8cd18-163">Video tutorial: Create a budget in the Azure portal</span></span>](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [<span data-ttu-id="8cd18-164">예산 보기 및 사용자 지정을 위한 필수 구성 요소</span><span class="sxs-lookup"><span data-stu-id="8cd18-164">Prerequisites for viewing and customizing budgets</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [<span data-ttu-id="8cd18-165">예산 만들기 및 관리</span><span class="sxs-lookup"><span data-stu-id="8cd18-165">Create and manage budgets</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [<span data-ttu-id="8cd18-166">Azure 작업 그룹 및 예산 API를 사용 하 여 자동화 구성</span><span class="sxs-lookup"><span data-stu-id="8cd18-166">Configure automation with Azure Action Groups and Budgets API</span></span>](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [<span data-ttu-id="8cd18-167">비용 알림을 사용 하 여 사용 현황 및 비용 모니터링</span><span class="sxs-lookup"><span data-stu-id="8cd18-167">Use cost alerts to monitor usage and spending</span></span>](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="8cd18-168">비용 관리 모범 사례</span><span class="sxs-lookup"><span data-stu-id="8cd18-168">Cost Management best practices</span></span>](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

<span data-ttu-id="8cd18-169">**자습서 동영상**</span><span class="sxs-lookup"><span data-stu-id="8cd18-169">**Tutorial videos**</span></span>

- [<span data-ttu-id="8cd18-170">Azure 포털에서 예산 만들기</span><span class="sxs-lookup"><span data-stu-id="8cd18-170">Create a budget in the Azure portal</span></span>](https://go.microsoft.com/fwlink/?linkid=2146761)
- [<span data-ttu-id="8cd18-171">예산 API 및 작업 그룹을 사용한 비용 관리</span><span class="sxs-lookup"><span data-stu-id="8cd18-171">Manage costs with the Budgets API and Action Groups</span></span>](https://go.microsoft.com/fwlink/?linkid=2147038)