---
title: 인증 라이브러리 작업
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897899"
---
# <a name="working-with-authentication-libraries"></a><span data-ttu-id="01ad6-102">인증 라이브러리 작업</span><span class="sxs-lookup"><span data-stu-id="01ad6-102">Working with Authentication Libraries</span></span>

<span data-ttu-id="01ad6-103">MSAL(Microsoft 인증 라이브러리) 문제를 해결하고 다음 권장 단계를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="01ad6-103">To resolve Microsoft Authentication Library (MSAL) issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="01ad6-104">**MSAL 작업**: [Microsoft ID 플랫폼 인증 라이브러리](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - 이 문서에서는 여러 응용 프로그램 유형에 대한 Microsoft 인증 라이브러리 지원을 보여 줍니다.</span><span class="sxs-lookup"><span data-stu-id="01ad6-104">**Working with MSAL**: [Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - This article shows Microsoft Authentication Library support for several application types.</span></span> <span data-ttu-id="01ad6-105">여기에는 라이브러리 소스 코드 링크, 앱 프로젝트의 패키지를 가져올 위치, 라이브러리가 사용자 로그인(인증), 보호된 웹 API(인증)에 대한 액세스를 지원하는지 여부 또는 둘 다 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="01ad6-105">It includes links to library source code; where to get the package for your app's project; and whether the library supports user sign-in (authentication), access to protected web APIs (authorization), or both.</span></span>

2. <span data-ttu-id="01ad6-106">**인증 문제 해결**: MSAL은 여러 응용 프로그램 시나리오에서 사용할 수 있도록 여러 인증 흐름을 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="01ad6-106">**Troubleshoot Authentication**: The MSAL supports several authentication flows for use in different application scenarios.</span></span> <span data-ttu-id="01ad6-107">클라이언트 응용 프로그램이 빌드되는 방식에 따라 MSAL은 Microsoft ID 플랫폼에서 지원되는 인증 흐름 중 하나 이상을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="01ad6-107">Depending on how your client application is built, the MSAL can use one or more of the authentication flows supported by the Microsoft identity platform.</span></span> <span data-ttu-id="01ad6-108">이러한 흐름은 여러 유형의 토큰과 인증 코드를 생성할 수 있으며, 이를 작동시키려면 서로 다른 토큰이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="01ad6-108">These flows can produce several types of tokens and authorization codes, and require different tokens to make them work.</span></span>

3. <span data-ttu-id="01ad6-109">**액세스 토큰**: [Microsoft ID 플랫폼 액세스 토큰](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - API에서 액세스 코튼 내부 클레임의 유효성을 검사하고 사용하는 방법을 알아봅니다.</span><span class="sxs-lookup"><span data-stu-id="01ad6-109">**Access Tokens**: [Microsoft identity platform access tokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Learn how your API can validate and use the claims inside an access token.</span></span> <span data-ttu-id="01ad6-110">이 게시물의 모든 문서(설명된 경우를 제외)는 등록한 API에 대해 발급된 토큰에만 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="01ad6-110">All documentation in this article, except where noted, applies only to tokens issued for APIs you've registered.</span></span> <span data-ttu-id="01ad6-111">Microsoft 소유 API용으로 발급된 토큰에는 적용되지 않으며 사용자가 생성한 API에 대해 Microsoft ID 플랫폼이 토큰을 발행하는 방법을 확인하는 데 이러한 토큰을 사용할 수도 없습니다.</span><span class="sxs-lookup"><span data-stu-id="01ad6-111">It does not apply to tokens issued for Microsoft-owned APIs, nor can those tokens be used to validate how the Microsoft identity platform will issue tokens for an API you create.</span></span>

<span data-ttu-id="01ad6-112">**ADAL(Azure Active Directory 인증 라이브러리)에 대한 지원 종료**</span><span class="sxs-lookup"><span data-stu-id="01ad6-112">**End of support for Azure Active Directory Authentication Library (ADAL)**</span></span>

- <span data-ttu-id="01ad6-113">**2020년 6월 30일부터** ADAL 및 Azure AD Graph에 새로운 기능이 추가되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="01ad6-113">**Starting June 30th, 2020,** we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="01ad6-114">기술 지원 및 보안 업데이트를 계속 제공하지만 기능 업데이트는 더 이상 제공하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="01ad6-114">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
- <span data-ttu-id="01ad6-115">**2022년 6월 30일부터** ADAL 및 Azure AD Graph에 대한 지원을 종료하고 더 이상 기술 지원이나 보안 업데이트를 제공하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="01ad6-115">**Starting June 30th, 2022,** we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>
- <span data-ttu-id="01ad6-116">기존 OS 버전에서 ADAL을 사용하는 앱은 이 시간 이후에도 계속 작동하지만 *기술 지원이나 보안 업데이트* 를 받지 못합니다.</span><span class="sxs-lookup"><span data-stu-id="01ad6-116">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>
- <span data-ttu-id="01ad6-117">이 시간 이후 Azure AD Graph를 사용하는 앱은 더 이상 Azure AD Graph 끝점에서 응답을 받지 못할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="01ad6-117">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="01ad6-118">**ADAL 마이그레이션**</span><span class="sxs-lookup"><span data-stu-id="01ad6-118">**ADAL Migration**</span></span>

- <span data-ttu-id="01ad6-119">최신 기능 및 보안 업데이트가 있는 MSAL로 업데이트하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="01ad6-119">We recommend updating to the MSAL, which has the latest features and security updates.</span></span>
- <span data-ttu-id="01ad6-120">Microsoft 앱을 사용하는 경우 Microsoft가 지원 종료시까지 MSAL로 응용 프로그램을 마이그레이션하고 있으며, MSAL의 지속적인 보안 및 기능 개선으로 혜택을 받을 수 있도록 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="01ad6-120">If you're using Microsoft apps, know that Microsoft is in the process of migrating its apps to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="01ad6-121">[ADAL FAQ를 읽어보세요](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="01ad6-121">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
2. <span data-ttu-id="01ad6-122">[플랫폼별로 앱을 마이그레이션하는 방법을 알아보세요](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span><span class="sxs-lookup"><span data-stu-id="01ad6-122">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span></span>
3. <span data-ttu-id="01ad6-123">앱 플랫폼 가이드를 읽은 후 추가 질문이 있는 경우 [azure-addal-declation] 태그가 있는 [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html)에 게시하거나 라이브러리의 GitHub 저장소에서 문제를 열 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="01ad6-123">If, after reading the guide for your app's platform, you have additional questions, you can post on [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) with the tag [azure-ad-adal-deprecation] or open an issue in library's GitHub repository.</span></span> <span data-ttu-id="01ad6-124">각 라이브러리의 참조 링크는 [MSAL 개요](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) 문서의 **언어 및 프레임워크** 섹션을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="01ad6-124">See the [Languages and frameworks](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) section of the **MSAL overview** article for links to each library's repo.</span></span>
4. <span data-ttu-id="01ad6-125">**어느 앱에서 ADAL을 사용하는지 이해하는 데 도움이 필요한 경우** 모든 앱의 소스 코드를 검토하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="01ad6-125">**If you need help understanding which of your apps use ADAL**, we recommend you review all of your apps' source code.</span></span> <span data-ttu-id="01ad6-126">해당되는 경우 ISV(독립 소프트웨어 벤더) 또는 앱 공급자에게 문의하세요.</span><span class="sxs-lookup"><span data-stu-id="01ad6-126">If applicable, reach out to any Independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="01ad6-127">또한 Microsoft 지원을 통해 테넌트에 있는 Microsoft가 아닌 모든 ADAL 앱 목록을 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="01ad6-127">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>







