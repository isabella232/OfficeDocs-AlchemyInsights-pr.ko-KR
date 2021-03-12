---
title: Microsoft Graph API 문제
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
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/29/2021
ms.locfileid: "50716200"
---
# <a name="microsoft-graph-api-issues"></a><span data-ttu-id="71cc8-102">Microsoft Graph API 문제</span><span class="sxs-lookup"><span data-stu-id="71cc8-102">Microsoft Graph API issues</span></span>

<span data-ttu-id="71cc8-103">이 항목은 여전히 Azure AD Graph API를 사용하는 개발자에게도 적용될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="71cc8-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="71cc8-104">그러나 모든  디렉터리, ID 및 액세스 관리 시나리오에 Microsoft Graph를 사용하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="71cc8-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="71cc8-105">**인증 또는 권한 부여 문제**</span><span class="sxs-lookup"><span data-stu-id="71cc8-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="71cc8-106">앱에서 Microsoft  Graph를 호출하는 토큰을 얻을 수 없는 경우 이 항목에 대한 자세한 도움말과 지원을 확인하려면 액세스 토큰(인증) Microsoft Graph 범주를 사용하는 데 문제가 있는 경우를 선택합니다. </span><span class="sxs-lookup"><span data-stu-id="71cc8-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="71cc8-107">앱에서 Microsoft Graph를 호출할 때 **401 또는 403** 권한 부여 오류가 발생하는 경우 액세스 거부 오류 보기(권한 **부여)** Microsoft Graph API 범주를 선택해 이 항목에 대한 보다 구체적인 도움말 및 지원을 얻습니다.</span><span class="sxs-lookup"><span data-stu-id="71cc8-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="71cc8-108">**Microsoft Graph를 사용하지만 어디서 시작해야 할지 잘 모르겠다**</span><span class="sxs-lookup"><span data-stu-id="71cc8-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

- [<span data-ttu-id="71cc8-109">Microsoft Graph 개요</span><span class="sxs-lookup"><span data-stu-id="71cc8-109">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="71cc8-110">Microsoft Graph의 ID 및 액세스 관리 개요</span><span class="sxs-lookup"><span data-stu-id="71cc8-110">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="71cc8-111">Microsoft Graph 앱 구축 시작</span><span class="sxs-lookup"><span data-stu-id="71cc8-111">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="71cc8-112">**Microsoft Graph 탐색기** - 테넌트 또는 데모 테넌트에서 Microsoft Graph API 테스트</span><span class="sxs-lookup"><span data-stu-id="71cc8-112">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="71cc8-113">**Microsoft Graph를 사용하지만 필요한 v1.0 디렉터리 API를 지원하나요?**</span><span class="sxs-lookup"><span data-stu-id="71cc8-113">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="71cc8-114">디렉터리, ID 및 액세스 관리에 권장되는 API는 Microsoft Graph입니다.</span><span class="sxs-lookup"><span data-stu-id="71cc8-114">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="71cc8-115">그러나 Azure AD Graph와 Microsoft Graph 간에는 여전히 몇 가지 간격이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="71cc8-115">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="71cc8-116">다음 문서를 검토하여 선택에 도움이 될 최신 차이점을 중점적으로 다듬습니다.</span><span class="sxs-lookup"><span data-stu-id="71cc8-116">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="71cc8-117">Azure AD Graph와 Microsoft Graph 간의 리소스 유형 차이</span><span class="sxs-lookup"><span data-stu-id="71cc8-117">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="71cc8-118">Azure AD Graph와 Microsoft Graph의 속성 차이</span><span class="sxs-lookup"><span data-stu-id="71cc8-118">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="71cc8-119">Azure AD와 Microsoft Graph의 메서드 차이</span><span class="sxs-lookup"><span data-stu-id="71cc8-119">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="71cc8-120">**호출하는 API가 작동하지 않습니다. 더 많은 테스트를 어디서 할 수 있나요?**</span><span class="sxs-lookup"><span data-stu-id="71cc8-120">**The API I am calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="71cc8-121">**Microsoft Graph 탐색기** - 테넌트 또는 데모 테넌트에서  Microsoft Graph API를 테스트하고 Microsoft Graph 탐색기에서 샘플 쿼리도 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="71cc8-121">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="71cc8-122">**내 앱이 너무 느리며 또한 스로틀링됩니다. 개선할 수 있는 기능**</span><span class="sxs-lookup"><span data-stu-id="71cc8-122">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="71cc8-123">시나리오에 따라 다양한 옵션을 사용하여 응용 프로그램의 실행을 높일 수 있으며, 경우에 따라 서비스에서 스로틀링하기 까다로우기 까다로우며(너무 많은 전화를 걸 때) 다양한 옵션을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="71cc8-123">Depending on your scenario, there are a variety of options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

- [<span data-ttu-id="71cc8-124">Microsoft Graph 모범 사례</span><span class="sxs-lookup"><span data-stu-id="71cc8-124">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="71cc8-125">일괄 처리 요청</span><span class="sxs-lookup"><span data-stu-id="71cc8-125">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="71cc8-126">델타 쿼리를 통해 변경 내용 추적</span><span class="sxs-lookup"><span data-stu-id="71cc8-126">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="71cc8-127">webhook을 통해 변경 내용에 대한 알림을 받을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="71cc8-127">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="71cc8-128">스로틀 지침</span><span class="sxs-lookup"><span data-stu-id="71cc8-128">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="71cc8-129">**오류 및 알려진 문제에 대한 자세한 내용은 어디에서 찾을 수 있나요?**</span><span class="sxs-lookup"><span data-stu-id="71cc8-129">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="71cc8-130">Microsoft Graph 오류 응답 정보</span><span class="sxs-lookup"><span data-stu-id="71cc8-130">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="71cc8-131">Microsoft Graph의 알려진 문제</span><span class="sxs-lookup"><span data-stu-id="71cc8-131">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="71cc8-132">**서비스 가용성 및 연결 상태를 어디에서 확인할 수 있나요?**</span><span class="sxs-lookup"><span data-stu-id="71cc8-132">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="71cc8-133">Microsoft Graph를 통해 액세스할 수 있는 서비스 가용성 및 연결성은 Microsoft Graph의 전반적인 가용성 및 성능에 영향을 줄 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="71cc8-133">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="71cc8-134">Azure Active Directory 서비스 상태의 경우 Azure 상태 페이지에 나열된 **보안 + ID** 서비스의 상태를 [확인합니다.](https://azure.microsoft.com/status/)</span><span class="sxs-lookup"><span data-stu-id="71cc8-134">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="71cc8-135">Microsoft Graph에 참여하는 Office 서비스의 경우 Office 서비스 상태 대시보드에 나열된 서비스의 [상태를 확인 합니다.](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="71cc8-135">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="71cc8-136">Microsoft Graph 권한 부여 오류는 여러 가지 문제로 인해 발생할 수 있습니다. 이로 인해 대부분 401 또는 403 오류가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="71cc8-136">Microsoft Graph authorization errors can be a result of several different issues, most of which generate a 401 or 403 error.</span></span> <span data-ttu-id="71cc8-137">예를 들어 다음이 모두 권한 부여 오류가 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="71cc8-137">For example, the following can all lead to authorization errors:</span></span>

- <span data-ttu-id="71cc8-138">잘못된 [액세스 토큰 획득 흐름](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span><span class="sxs-lookup"><span data-stu-id="71cc8-138">Incorrect [access token acquisition flows](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span></span>
- <span data-ttu-id="71cc8-139">잘못된 [권한 범위 구성](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span><span class="sxs-lookup"><span data-stu-id="71cc8-139">Poorly configured [permission scopes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span></span>
- <span data-ttu-id="71cc8-140">[동의](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent) 부족</span><span class="sxs-lookup"><span data-stu-id="71cc8-140">Lack of [consent](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span></span>

<span data-ttu-id="71cc8-141">\**_ADAL(Azure Active Directory 인증 라이브러리) 및 AZure AD 그래프 API(AAD Graph) 지원 종료_* _</span><span class="sxs-lookup"><span data-stu-id="71cc8-141">\**_End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)_* _</span></span>

<span data-ttu-id="71cc8-142">_\*2020년 6월 30일\*\*부터는 더 이상 ADAL 및 Azure AD Graph에 새 기능을 추가하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="71cc8-142">_\*Starting June 30th, 2020\*\*, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="71cc8-143">기술 지원 및 보안 업데이트를 계속 제공하지만 기능 업데이트는 더 이상 제공하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="71cc8-143">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="71cc8-144">**2022년 6월 30일부터** ADAL 및 Azure AD Graph에 대한 지원이 종료될 예정으로, 더 이상 기술 지원 또는 보안 업데이트를 제공하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="71cc8-144">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="71cc8-145">기존 OS 버전에서 ADAL을 사용하는 앱은 이 시간 이후에도 계속 작동하지만 기술 지원 또는 보안 업데이트는 받을 *수 없습니다.*</span><span class="sxs-lookup"><span data-stu-id="71cc8-145">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="71cc8-146">이 시간이 지난 후 Azure AD Graph를 사용하는 앱은 더 이상 Azure AD Graph 끝점에서 응답을 받지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="71cc8-146">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="71cc8-147">**ADAL 마이그레이션**</span><span class="sxs-lookup"><span data-stu-id="71cc8-147">**ADAL Migration**</span></span>

<span data-ttu-id="71cc8-148">최신 기능 및 보안 업데이트가 있는 [MSAL(Microsoft Authentication Library)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)로 업데이트하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="71cc8-148">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="71cc8-149">Microsoft 앱을 사용하는 경우 Microsoft가 지원 종료 기한까지 응용 프로그램을 MSAL로 마이그레이션하는 중이라는 것을 알고 MSAL의 지속적인 보안 및 기능 개선을 통해 혜택을 받을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="71cc8-149">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="71cc8-150">ADAL FAQ 읽기</span><span class="sxs-lookup"><span data-stu-id="71cc8-150">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="71cc8-151">플랫폼별로 앱을 마이그레이션하는 방법 알아보기</span><span class="sxs-lookup"><span data-stu-id="71cc8-151">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="71cc8-152">ADAL을 사용하는 앱을 이해하는 데 도움이 필요한 경우 모든 앱의 소스 코드를 검토하고 해당하는 경우 ISV 또는 앱 공급자에게 도움을 드리는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="71cc8-152">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="71cc8-153">또한 Microsoft 지원을 통해 테넌트에 있는 Microsoft가 아닌 모든 ADAL 앱 목록을 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="71cc8-153">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="71cc8-154">**AAD 그래프 마이그레이션**</span><span class="sxs-lookup"><span data-stu-id="71cc8-154">**AAD Graph Migration**</span></span>

<span data-ttu-id="71cc8-155">Azure AD Graph를 사용하는 응용 프로그램의 경우 지침에 따라 Azure AD Graph 앱을 [Microsoft Graph로 마이그레이션합니다.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)</span><span class="sxs-lookup"><span data-stu-id="71cc8-155">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. <span data-ttu-id="71cc8-156">[마이그레이션 점검표를 통해 시작 지점 제공](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)</span><span class="sxs-lookup"><span data-stu-id="71cc8-156">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span>
2. <span data-ttu-id="71cc8-157">Azure 앱 등록 포털에 AAD 그래프를 사용하는 응용 프로그램이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="71cc8-157">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="71cc8-158">모든 앱의 소스 코드를 검토하고 해당되는 경우 ISV 또는 앱 공급자에게 문의하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="71cc8-158">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="71cc8-159">Microsoft 지원은 테넌트의 모든 AAD Graph 사용 목록을 제공할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="71cc8-159">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="71cc8-160">앱에서 Microsoft Graph의 데이터에 액세스하려면 사용자 또는 관리자가 동의 프로세스를 통해 올바른 사용 권한을 부여해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="71cc8-160">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="71cc8-161">[Microsoft Graph 사용 권한 참조에는](https://docs.microsoft.com/graph/permissions-reference) 각 주요 Microsoft Graph API 집합과 연결된 사용 권한이 나열됩니다.</span><span class="sxs-lookup"><span data-stu-id="71cc8-161">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="71cc8-162">또한 사용 권한을 사용하는 방법에 대한 지침도 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="71cc8-162">It also provides guidance about how to use the permissions.</span></span>
