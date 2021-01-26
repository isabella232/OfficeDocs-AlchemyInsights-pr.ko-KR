---
title: Microsoft Graph API 쿼리
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
- "9004345"
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950777"
---
# <a name="querying-the-microsoft-graph-api"></a><span data-ttu-id="19b2e-102">Microsoft Graph API 쿼리</span><span class="sxs-lookup"><span data-stu-id="19b2e-102">Querying the Microsoft Graph API</span></span>

<span data-ttu-id="19b2e-103">이 항목은 여전히 Azure AD Graph API를 사용하는 개발자에게도 적용될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="19b2e-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="19b2e-104">그러나 모든  디렉터리, ID 및 액세스 관리 시나리오에 Microsoft Graph를 사용하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="19b2e-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="19b2e-105">**인증 또는 권한 부여 문제**</span><span class="sxs-lookup"><span data-stu-id="19b2e-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="19b2e-106">앱에서 Microsoft  Graph를 호출하는 토큰을 얻을 수 없는 경우 이 항목에 대한 보다 구체적인 도움말 및 지원을 확인하려면 액세스 **토큰(인증)** Microsoft Graph 범주를 사용하는 데 문제가 있는 경우 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="19b2e-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="19b2e-107">앱에서 Microsoft Graph를 호출할 때 **401 또는 403** 권한 부여 오류가 발생하는 경우 액세스 거부 오류(권한 **부여)** Microsoft Graph API 범주를 선택해 이 항목에 대한 보다 구체적인 도움말 및 지원을 얻습니다.</span><span class="sxs-lookup"><span data-stu-id="19b2e-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="19b2e-108">**Microsoft Graph를 사용하지만 어디서 시작해야 할지 잘 모르겠다.**</span><span class="sxs-lookup"><span data-stu-id="19b2e-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

<span data-ttu-id="19b2e-109">Microsoft Graph에 대한 자세한 내용은 다음을 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="19b2e-109">To learn more about Microsoft Graph, see:</span></span>

- [<span data-ttu-id="19b2e-110">Microsoft Graph 개요</span><span class="sxs-lookup"><span data-stu-id="19b2e-110">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="19b2e-111">Microsoft Graph의 ID 및 액세스 관리 개요</span><span class="sxs-lookup"><span data-stu-id="19b2e-111">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="19b2e-112">Microsoft Graph 앱 구축 시작</span><span class="sxs-lookup"><span data-stu-id="19b2e-112">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="19b2e-113">**Microsoft Graph 탐색기** - 테넌트 또는 데모 테넌트에서 Microsoft Graph API 테스트</span><span class="sxs-lookup"><span data-stu-id="19b2e-113">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="19b2e-114">**Microsoft Graph를 사용하지만 필요한 v1.0 디렉터리 API를 지원하나요?**</span><span class="sxs-lookup"><span data-stu-id="19b2e-114">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="19b2e-115">Microsoft Graph는 디렉터리, ID 및 액세스 관리에 권장되는 API입니다.</span><span class="sxs-lookup"><span data-stu-id="19b2e-115">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="19b2e-116">그러나 Azure AD Graph와 Microsoft Graph에서 가능한 간격은 여전히 몇 가지가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="19b2e-116">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="19b2e-117">다음 문서를 검토하여 선택한 데 도움이 될 최신 차이점을 중점적으로 다수 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="19b2e-117">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="19b2e-118">Azure AD Graph와 Microsoft Graph 간의 리소스 유형 차이</span><span class="sxs-lookup"><span data-stu-id="19b2e-118">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="19b2e-119">Azure AD Graph와 Microsoft Graph의 속성 차이</span><span class="sxs-lookup"><span data-stu-id="19b2e-119">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="19b2e-120">Azure AD와 Microsoft Graph의 메서드 차이</span><span class="sxs-lookup"><span data-stu-id="19b2e-120">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="19b2e-121">**사용자 개체를 *쿼리할* 때 많은 속성이 누락되었습니다.**</span><span class="sxs-lookup"><span data-stu-id="19b2e-121">**When I query the *user* object, many of its properties are missing**</span></span>

<span data-ttu-id="19b2e-122">`GET https://graph.microsoft.com/v1.0/users`Microsoft Graph에서 반환할 기본 사용자 속성 집합을 자동으로  선택하면 11개 속성만 반환됩니다.</span><span class="sxs-lookup"><span data-stu-id="19b2e-122">`GET https://graph.microsoft.com/v1.0/users` only returns 11 properties, as Microsoft Graph auto-selects a default set of *user* properties to return.</span></span> <span data-ttu-id="19b2e-123">다른 사용자  속성이 필요한 경우 $select 속성을 선택하십시오.</span><span class="sxs-lookup"><span data-stu-id="19b2e-123">If you need other *user* properties, use $select to pick the properties your application needs.</span></span> <span data-ttu-id="19b2e-124">먼저 Microsoft **Graph 탐색기에서 사용해** 보아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="19b2e-124">Try it out in **Microsoft Graph Explorer** first.</span></span>

<span data-ttu-id="19b2e-125">**일부 사용자 속성 값은 설정되어 있는 것을 알지만 *null입니다.***</span><span class="sxs-lookup"><span data-stu-id="19b2e-125">**Some user property values are *null* even though I know they are set**</span></span>

<span data-ttu-id="19b2e-126">가장 가능성이 높은 설명은 응용 프로그램에 *User.ReadBasic.All 권한이 부여된 것입니다.*</span><span class="sxs-lookup"><span data-stu-id="19b2e-126">The most likely explanation is that the application had been granted the *User.ReadBasic.All* permission.</span></span> <span data-ttu-id="19b2e-127">이렇게 하면 응용 프로그램에서 제한된 사용자 속성 집합을 읽을 수 있습니다. 다른 모든 속성은 이전에 설정한 경우에도 null로 반환됩니다.</span><span class="sxs-lookup"><span data-stu-id="19b2e-127">This allows the application to read a limited set of user properties, returning all other properties as null even if they have been previously set.</span></span> <span data-ttu-id="19b2e-128">대신 *User.Read.All* 권한을 응용 프로그램에 부여합니다.</span><span class="sxs-lookup"><span data-stu-id="19b2e-128">Try granting the application *User.Read.All* permission instead.</span></span>

<span data-ttu-id="19b2e-129">자세한 내용은 Microsoft Graph 사용자 [권한을 참조하세요.](https://docs.microsoft.com/graph/permissions-reference#user-permissions)</span><span class="sxs-lookup"><span data-stu-id="19b2e-129">For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span></span>

<span data-ttu-id="19b2e-130">**OData 쿼리 매개 변수를 사용하여 요청의 데이터를 필터링하는 데 문제가 있습니다.**</span><span class="sxs-lookup"><span data-stu-id="19b2e-130">**I'm having trouble using OData query parameters to filter data in my requests**</span></span>

<span data-ttu-id="19b2e-131">Microsoft Graph는 광범위한 OData 쿼리 매개 변수를 지원하기는 하지만 이러한 매개 변수 중 상당수는 Microsoft Graph의 디렉터리 *서비스(디렉터리Object에서* 상속하는 리소스)에서 완전히 지원되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="19b2e-131">While Microsoft Graph supports a wide range of the OData query parameters, many of those parameters are not fully supported by directory services (resources that inherit from *directoryObject*) in Microsoft Graph.</span></span> <span data-ttu-id="19b2e-132">Azure AD Graph에 있는 동일한 제한은 Microsoft Graph에서 대부분 지속됩니다.</span><span class="sxs-lookup"><span data-stu-id="19b2e-132">The same limitations that were present in Azure AD Graph persist for the most part in Microsoft Graph:</span></span>

1. <span data-ttu-id="19b2e-133">**지원되지** 않는 값: *null* $count $search, $filter 및 *지원되지* 않습니다.</span><span class="sxs-lookup"><span data-stu-id="19b2e-133">**Not supported**: $count, $search, and $filter on *null* or *not null* values</span></span>
2. <span data-ttu-id="19b2e-134">**지원되지**$filter 속성에 대한 정보 표시(필터링 가능한 속성에 대한 리소스 항목 참조)</span><span class="sxs-lookup"><span data-stu-id="19b2e-134">**Not supported**: $filter on certain properties (see resource topics on which properties are filterable)</span></span>
3. <span data-ttu-id="19b2e-135">**지원되지** 않는 경우: 동시에 파이징, 필터링 및 정렬</span><span class="sxs-lookup"><span data-stu-id="19b2e-135">**Not supported**: paging, filtering, and sorting at the same time</span></span>
4. <span data-ttu-id="19b2e-136">**지원되지** 않습니다. 관계에 대한 필터링.</span><span class="sxs-lookup"><span data-stu-id="19b2e-136">**Not supported**: filtering on a relationship.</span></span> <span data-ttu-id="19b2e-137">예 - 영국에 있는 엔지니어링 그룹의 모든 구성원을 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="19b2e-137">For example - find all members of the engineering group that are in the UK.</span></span>
5. <span data-ttu-id="19b2e-138">**부분 지원**: $orderby(displayName 및 userPrincipalName만 해당) 및  *그룹에서 지원*</span><span class="sxs-lookup"><span data-stu-id="19b2e-138">**Partial support**: $orderby on *user* (displayName and userPrincipalName only) and *group*</span></span>
6. <span data-ttu-id="19b2e-139">**부분** 지원 : $filter *(eq,* *startwith* 또는 제한) 지원, $expand(단일 개체의 관계 확장은 모든 관계는 반환되지만 개체의 관계 컬렉션 확장은 제한)</span><span class="sxs-lookup"><span data-stu-id="19b2e-139">**Partial support**: $filter (supports only *eq*, *startswith*, *or*, *and*, and limited *any*) support, $expand (expanding a single object's relationships returns all relationships, but expanding a collection of objects' relationships is limited)</span></span>

<span data-ttu-id="19b2e-140">자세한 내용은 쿼리 매개 [변수를 사용하여 응답 사용자 지정을 참조하세요.](https://docs.microsoft.com/graph/query-parameters)</span><span class="sxs-lookup"><span data-stu-id="19b2e-140">For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span></span>

<span data-ttu-id="19b2e-141">**호출하는 API가 작동하지 않습니다. 더 많은 테스트를 할 수 있는 곳은 어디인가요?**</span><span class="sxs-lookup"><span data-stu-id="19b2e-141">**The API I'm calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="19b2e-142">**Microsoft Graph 탐색기** - 테넌트 또는 데모 테넌트에서  Microsoft Graph API를 테스트하고 Microsoft Graph 탐색기에서 샘플 쿼리도 체크 아웃합니다.</span><span class="sxs-lookup"><span data-stu-id="19b2e-142">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="19b2e-143">**데이터를 쿼리할 때 불완전한 데이터 집합이 다시 있는 것 같습니다.**</span><span class="sxs-lookup"><span data-stu-id="19b2e-143">**When I query for data it seems like I get an incomplete data set back**</span></span>

<span data-ttu-id="19b2e-144">사용자와 같은 컬렉션을 쿼리하는 경우 Microsoft Graph에서는 서버 쪽 페이지 제한을 사용하여 결과가 항상 기본 페이지 크기로 반환됩니다. </span><span class="sxs-lookup"><span data-stu-id="19b2e-144">If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size.</span></span> <span data-ttu-id="19b2e-145">앱은 항상 서비스에서 반환된 컬렉션을 페이지로 이동해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="19b2e-145">Your app should always expect to page through collections returned from the service.</span></span>

<span data-ttu-id="19b2e-146">자세한 내용은 다음을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="19b2e-146">For more information, see:</span></span>

- [<span data-ttu-id="19b2e-147">Microsoft Graph 모범 사례</span><span class="sxs-lookup"><span data-stu-id="19b2e-147">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="19b2e-148">앱에서 Microsoft Graph 데이터 파이징</span><span class="sxs-lookup"><span data-stu-id="19b2e-148">Paging Microsoft Graph data in your app</span></span>](https://docs.microsoft.com/graph/paging)

<span data-ttu-id="19b2e-149">**내 앱이 너무 느리며 또한 스로틀링되고 있습니다. 개선할 수 있는 기능**</span><span class="sxs-lookup"><span data-stu-id="19b2e-149">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="19b2e-150">시나리오에 따라 응용 프로그램의 실행을 보다 잘 수행하기 위해 다양한 옵션을 사용할 수 있으며, 경우에 따라 서비스로의 스로틀링을 덜 수 있습니다(너무 많은 호출을 하는 경우).</span><span class="sxs-lookup"><span data-stu-id="19b2e-150">Depending on your scenario, there are a variety of different options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

<span data-ttu-id="19b2e-151">자세한 내용은 다음을 참조하세요:</span><span class="sxs-lookup"><span data-stu-id="19b2e-151">To learn more, see:</span></span>

- [<span data-ttu-id="19b2e-152">Microsoft Graph 모범 사례</span><span class="sxs-lookup"><span data-stu-id="19b2e-152">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="19b2e-153">요청 일괄 처리</span><span class="sxs-lookup"><span data-stu-id="19b2e-153">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="19b2e-154">델타 쿼리를 통해 변경 내용 추적</span><span class="sxs-lookup"><span data-stu-id="19b2e-154">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="19b2e-155">webhook을 통해 변경 내용 알림을 받을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="19b2e-155">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="19b2e-156">스로틀 지침</span><span class="sxs-lookup"><span data-stu-id="19b2e-156">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="19b2e-157">**오류 및 알려진 문제에 대한 자세한 내용은 어디에서 찾을 수 있나요?**</span><span class="sxs-lookup"><span data-stu-id="19b2e-157">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="19b2e-158">Microsoft Graph 오류 응답 정보</span><span class="sxs-lookup"><span data-stu-id="19b2e-158">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="19b2e-159">Microsoft Graph의 알려진 문제</span><span class="sxs-lookup"><span data-stu-id="19b2e-159">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="19b2e-160">**서비스 가용성 및 연결 상태를 어디에서 확인할 수 있나요?**</span><span class="sxs-lookup"><span data-stu-id="19b2e-160">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="19b2e-161">Microsoft Graph를 통해 액세스할 수 있는 서비스 가용성 및 연결은 Microsoft Graph의 전반적인 가용성 및 성능에 영향을 줄 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="19b2e-161">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="19b2e-162">Azure Active Directory 서비스 상태의 경우 Azure 상태 페이지에 나열된 **보안 + ID** 서비스의 상태를 [확인합니다.](https://azure.microsoft.com/status/)</span><span class="sxs-lookup"><span data-stu-id="19b2e-162">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="19b2e-163">Microsoft Graph에 참여하는 Office 서비스의 경우 Office 서비스 상태 대시보드에 나열된 서비스의 [상태를 검사합니다.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="19b2e-163">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
