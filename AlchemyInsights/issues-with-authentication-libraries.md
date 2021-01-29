---
title: 인증 라이브러리 관련 문제
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
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50037217"
---
# <a name="issues-with-authentication-libraries"></a><span data-ttu-id="b49c7-102">인증 라이브러리 관련 문제</span><span class="sxs-lookup"><span data-stu-id="b49c7-102">Issues with Authentication Libraries</span></span>

1. <span data-ttu-id="b49c7-103">[Microsoft ID 플랫폼 인증 라이브러리에는](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) Microsoft에서 지원되는 호환되는 클라이언트 및 미들웨어 라이브러리가 나열됩니다.</span><span class="sxs-lookup"><span data-stu-id="b49c7-103">[Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) lists Microsoft-supported and compatible client and middleware libraries.</span></span>
2. <span data-ttu-id="b49c7-104">MSAL(Microsoft 인증 라이브러리)은 [](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) 다양한 응용 프로그램 시나리오에서 사용할 수 있는 몇 가지 인증 흐름을 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="b49c7-104">The Microsoft Authentication Library (MSAL) supports several [authentication flows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) for use in different application scenarios.</span></span>
3. <span data-ttu-id="b49c7-105">토큰을 인증하고 획득하기 위해 코드에서 새 공용 또는 기밀 클라이언트 응용 프로그램을 초기화합니다.</span><span class="sxs-lookup"><span data-stu-id="b49c7-105">To authenticate and acquire tokens, you initialize a new public or confidential client application in your code.</span></span> <span data-ttu-id="b49c7-106">MSAL(Microsoft 인증 라이브러리)에서 클라이언트 앱을 초기화할 때 몇 가지 구성 옵션을 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b49c7-106">You can set several configuration options when you initialize the client app in the Microsoft Authentication Library (MSAL).</span></span> <span data-ttu-id="b49c7-107">자세한 내용은 응용 프로그램 구성 [옵션을 참조하세요.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)</span><span class="sxs-lookup"><span data-stu-id="b49c7-107">To learn more, see [Application configuration options](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span></span>

<span data-ttu-id="b49c7-108">**Azure ADAL(Active Directory 인증 라이브러리) 및 Azure AD Graph API(AAD Graph)에 대한 지원 종료**</span><span class="sxs-lookup"><span data-stu-id="b49c7-108">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="b49c7-109">**2020년 6월 30일부터** 더 이상 ADAL 및 Azure AD Graph에 새로운 기능이 추가되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="b49c7-109">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="b49c7-110">기술 지원 및 보안 업데이트를 계속 제공하지만 기능 업데이트는 더 이상 제공하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="b49c7-110">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="b49c7-111">**2022년 6월 30일부터** ADAL 및 Azure AD Graph에 대한 지원이 종료될 예정으로, 더 이상 기술 지원 또는 보안 업데이트를 제공하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="b49c7-111">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="b49c7-112">기존 OS 버전에서 ADAL을 사용하는 앱은 이 시간 이후에도 계속 작동하지만 기술 지원 또는 보안 업데이트는 *제공되지 않습니다.*</span><span class="sxs-lookup"><span data-stu-id="b49c7-112">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="b49c7-113">이 시간 이후 Azure AD Graph를 사용하는 앱은 더 이상 Azure AD Graph 끝점에서 응답을 수신하지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b49c7-113">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="b49c7-114">**ADAL 마이그레이션**</span><span class="sxs-lookup"><span data-stu-id="b49c7-114">**ADAL Migration**</span></span>

<span data-ttu-id="b49c7-115">최신 기능 및 보안 업데이트가 있는 [MSAL(Microsoft Authentication Library)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)로 업데이트하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="b49c7-115">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="b49c7-116">Microsoft 앱을 사용하는 경우 Microsoft가 지원 종료 기한까지 MSAL로 응용 프로그램을 마이그레이션하는 중이라는 사실에 유의하여 MSAL의 지속적인 보안 및 기능 개선을 활용하도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="b49c7-116">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they will benefit from MSAL's ongoing security and feature improvements.</span></span>

<span data-ttu-id="b49c7-117">자세한 내용은 다음을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b49c7-117">For more information, see:</span></span>

1. [<span data-ttu-id="b49c7-118">ADAL FAQ 읽기</span><span class="sxs-lookup"><span data-stu-id="b49c7-118">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="b49c7-119">플랫폼별로 앱을 마이그레이션하는 방법 알아보기</span><span class="sxs-lookup"><span data-stu-id="b49c7-119">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="b49c7-120">ADAL을 사용하는 앱을 이해하는 데 도움이 필요한 경우 모든 앱의 소스 코드를 검토하는 것이 좋습니다. 해당하는 경우 ISV 또는 앱 공급자에게 연결합니다.</span><span class="sxs-lookup"><span data-stu-id="b49c7-120">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="b49c7-121">또한 Microsoft 지원을 통해 테넌트에 있는 Microsoft가 아닌 모든 ADAL 앱 목록을 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b49c7-121">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="b49c7-122">**AAD 그래프 마이그레이션**</span><span class="sxs-lookup"><span data-stu-id="b49c7-122">**AAD Graph Migration**</span></span>

<span data-ttu-id="b49c7-123">Azure AD Graph를 사용하는 응용 프로그램의 경우 지침에 따라 Azure AD Graph 앱을 [Microsoft Graph로 마이그레이션합니다.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)</span><span class="sxs-lookup"><span data-stu-id="b49c7-123">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. [<span data-ttu-id="b49c7-124">마이그레이션 검사 목록은 시작 지점을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="b49c7-124">Our migration checklist provides a getting started point.</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. <span data-ttu-id="b49c7-125">Azure 앱 등록 포털에 AAD 그래프를 사용하는 응용 프로그램이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="b49c7-125">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="b49c7-126">모든 앱의 소스 코드를 검토하고 해당되는 경우 ISV 또는 앱 공급자에게 문의하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="b49c7-126">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="b49c7-127">Microsoft 지원 서비스에서 테넌트의 모든 AAD Graph 사용 목록을 제공할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b49c7-127">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="b49c7-128">앱에서 Microsoft Graph의 데이터에 액세스하려면 사용자 또는 관리자가 동의 프로세스를 통해 올바른 사용 권한을 부여해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b49c7-128">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="b49c7-129">Microsoft Graph 사용 권한 [참조에는](https://docs.microsoft.com/graph/permissions-reference) 각 주요 Microsoft Graph API 집합과 연결된 사용 권한이 나열됩니다.</span><span class="sxs-lookup"><span data-stu-id="b49c7-129">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="b49c7-130">또한 사용 권한을 사용하는 방법에 대한 지침도 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="b49c7-130">It also provides guidance about how to use the permissions.</span></span>
