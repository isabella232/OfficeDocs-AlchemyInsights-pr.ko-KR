---
title: 인증 문제
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7748"
- "9004339"
ms.openlocfilehash: 2f413e863e6aa23548e425de5901f8158e1d48ab
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49976855"
---
# <a name="authentication-issues"></a><span data-ttu-id="b1d62-102">인증 문제</span><span class="sxs-lookup"><span data-stu-id="b1d62-102">Authentication issues</span></span>

<span data-ttu-id="b1d62-103">**Azure AD(Azure Active Directory) STS(보안 토큰 서비스)에서 반환되는 AADS 오류 코드에 대한 정보를 찾고 계신가요?**</span><span class="sxs-lookup"><span data-stu-id="b1d62-103">**Looking for information about the AADSTS error codes that are returned from the Azure Active Directory (Azure AD) security token service (STS)?**</span></span> <span data-ttu-id="b1d62-104">AADSTS 오류 설명, 수정 및 제안된 해결 방법을 찾으려면 [Azure AD 인증 및 인증 오류 코드](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b1d62-104">See [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>

<span data-ttu-id="b1d62-105">인증 오류는 401 또는 403 오류를 생성하는 여러 가지 문제로 인해 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-105">Authorization errors can be a result of several different issues, most of which generate a 401 or 403 error.</span></span> <span data-ttu-id="b1d62-106">예를 들어 다음과 같은 문제가 모두 권한 부여 오류로 이어질 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-106">For example, the following issues can all lead to authorization errors:</span></span>

- <span data-ttu-id="b1d62-107">잘못된 [액세스 토큰 획득 흐름](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization)</span><span class="sxs-lookup"><span data-stu-id="b1d62-107">Incorrect [access token acquisition flows](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization)</span></span> 
- <span data-ttu-id="b1d62-108">잘못된 [권한 범위 구성](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)</span><span class="sxs-lookup"><span data-stu-id="b1d62-108">Poorly configured [permission scopes](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)</span></span> 
- <span data-ttu-id="b1d62-109">[동의](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent) 부족</span><span class="sxs-lookup"><span data-stu-id="b1d62-109">Lack of [consent](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)</span></span>

<span data-ttu-id="b1d62-110">일반적인 권한 부여 오류를 해결하려면 수신되는 오류와 가장 일치하는 아래 단계를 시도해 보세요.</span><span class="sxs-lookup"><span data-stu-id="b1d62-110">To resolve common authorization errors, try the steps provided below which most closely match the error you are receiving.</span></span> <span data-ttu-id="b1d62-111">수신 중인 오류에 대해 둘 이상의 단계가 적용될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-111">More than one step may apply for an error you are receiving.</span></span>

<span data-ttu-id="b1d62-112">**401 Unauthorized error: 토큰이 유효한가요?**</span><span class="sxs-lookup"><span data-stu-id="b1d62-112">**401 Unauthorized error: Is your token valid?**</span></span>

<span data-ttu-id="b1d62-113">앱이 요청의 일부로 Microsoft Graph에 유효한 액세스 토큰을 제공하고 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-113">Ensure that your app is presenting a valid access token to Microsoft Graph as part of the request.</span></span> <span data-ttu-id="b1d62-114">이 오류는 종종 액세스 토큰이 HTTP 인증 요청 헤더에 없거나 토큰이 잘못되었거나 만료되었음을 의미합니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-114">This error often means that the access token may be missing in the HTTP authenticate request header or that the token is invalid or has expired.</span></span> <span data-ttu-id="b1d62-115">액세스 토큰 획득에 MSAL(Microsoft Authentication Library)을 사용하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-115">We strongly recommend that you use the Microsoft Authentication Library (MSAL) for access token acquisition.</span></span> <span data-ttu-id="b1d62-116">또한 개인 Microsoft 계정에 부여된 위임 액세스 토큰을 사용하여 회사 또는 학교 계정(조직 계정)만 지원하는 API에 액세스하려고 하면 이 오류가 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-116">Additionally, this error may occur if you try to use a delegated access token granted to a personal Microsoft account to access an API that only supports work or school accounts (organizational accounts).</span></span>

<span data-ttu-id="b1d62-117">**403 Forbidden error: 올바른 권한 세트를 선택했나요?**</span><span class="sxs-lookup"><span data-stu-id="b1d62-117">**403 Forbidden error: Have you chosen the right set of permissions?**</span></span>

<span data-ttu-id="b1d62-118">앱에서 호출하는 Microsoft Graph API를 기반으로 올바른 권한 집합을 요청했는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-118">Ensure that you have requested the correct set of permissions based on the Microsoft Graph APIs your app calls.</span></span> <span data-ttu-id="b1d62-119">권장 최소 권한 사용 권한은 모든 Microsoft Graph API 참조 방법 항목에서 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-119">Recommended least-privileged permissions are provided in all the Microsoft Graph API reference method topics.</span></span> <span data-ttu-id="b1d62-120">또한 이러한 권한은 사용자 또는 관리자가 응용 프로그램에 부여해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-120">Additionally, those permissions must be granted to the application by a user or an administrator.</span></span> <span data-ttu-id="b1d62-121">권한 부여는 일반적으로 동의 페이지 또는 Azure Portal 응용 프로그램 등록 블레이드의 사용을 통해 이루어집니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-121">Granting permissions normally happens through a consent page or usage of the Azure Portal application registration blade.</span></span> <span data-ttu-id="b1d62-122">응용 프로그램에 대한 **설정** 블레이드에서 **필수 권한** 을 클릭하고 **권한 허용** 을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-122">From the **Settings** blade for the application, click **Required Permissions**, and then click **Grant Permissions**.</span></span> <span data-ttu-id="b1d62-123">자세한 내용은 다음을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b1d62-123">For more information, see:</span></span>

- [<span data-ttu-id="b1d62-124">Microsoft Graph 사용 권한</span><span class="sxs-lookup"><span data-stu-id="b1d62-124">Microsoft Graph permissions</span></span>](https://docs.microsoft.com/graph/permissions-reference) 
- [<span data-ttu-id="b1d62-125">Azure AD 사용 권한 및 동의 이해</span><span class="sxs-lookup"><span data-stu-id="b1d62-125">Understanding Azure AD permissions and consent</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

<span data-ttu-id="b1d62-126">**403 Forbidden error: 앱에서 선택한 권한과 일치하는 토큰을 획득했나요?**</span><span class="sxs-lookup"><span data-stu-id="b1d62-126">**403 Forbidden error: Did your app acquire a token to match chosen permissions?**</span></span>

<span data-ttu-id="b1d62-127">요청하거나 부여된 권한 유형이 앱에서 획득한 액세스 토큰 유형과 일치하는지 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="b1d62-127">Ensure that the types of permissions requested or granted match the type of access token that your app acquires.</span></span> <span data-ttu-id="b1d62-128">앱 사용 권한을 요청 및 부여하지만 클라이언트 자격 증명 흐름 토큰 대신 위임된 대화형 코드 흐름 토큰을 사용하거나, 위임된 사용 권한을 요청 및 부여하지만 위임된 코드 흐름 토큰 대신 클라이언트 자격 증명 흐름 토큰을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-128">You might be requesting and granting app permissions but using delegated interactive code flow tokens instead of client credential flow tokens, or requesting and granting delegated permissions but using client credential flow tokens instead of delegated code flow tokens.</span></span>

<span data-ttu-id="b1d62-129">토큰 수집과 관련된 자세한 내용은 다음을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b1d62-129">For more information related to acquiring tokens, see:</span></span>

- [<span data-ttu-id="b1d62-130">사용자 및 위임된 사용 권한을 대신하여 액세스 권한 부여</span><span class="sxs-lookup"><span data-stu-id="b1d62-130">Get access on behalf of users and delegated permissions</span></span>](https://docs.microsoft.com/graph/auth-v2-user) 
- [<span data-ttu-id="b1d62-131">Azure AD v2.0 - OAuth 2.0 인증 코드 흐름</span><span class="sxs-lookup"><span data-stu-id="b1d62-131">Azure AD v2.0 - OAuth 2.0 authorization code flow</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [<span data-ttu-id="b1d62-132">사용자(데몬 서비스) 및 응용 프로그램 사용 권한 없이 액세스 가능</span><span class="sxs-lookup"><span data-stu-id="b1d62-132">Get access without a user (daemon service) and application permissions</span></span>](https://docs.microsoft.com/graph/auth-v2-service) 
- [<span data-ttu-id="b1d62-133">Azure AD v2.0 - OAuth 2.0 클라이언트 자격 증명 흐름</span><span class="sxs-lookup"><span data-stu-id="b1d62-133">Azure AD v2.0 - OAuth 2.0 client credentials flow</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

<span data-ttu-id="b1d62-134">**403 Forbidden error: 암호 재설정**</span><span class="sxs-lookup"><span data-stu-id="b1d62-134">**403 Forbidden error: Resetting password**</span></span>

<span data-ttu-id="b1d62-135">현재 사용자 암호를 재설정할 수 있는 응용 프로그램 권한 데몬 서비스 대 서비스 권한이 없습니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-135">Currently, there are no application permission daemon service-to-service permissions that allow resetting user passwords.</span></span> <span data-ttu-id="b1d62-136">이러한 API는 로그인한 관리자가 있는 대화형 위임 코드 흐름만 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-136">These APIs are only supported using the interactive delegated code flows with a signed-in administrator.</span></span> <span data-ttu-id="b1d62-137">자세한 내용은 [Microsoft Graph 사용 권한](https://docs.microsoft.com/graph/permissions-reference)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b1d62-137">For more information, see [Microsoft Graph permissions](https://docs.microsoft.com/graph/permissions-reference).</span></span>

<span data-ttu-id="b1d62-138">**403 Forbidden: 사용자에게 액세스 권한이 있으며 라이선스가 부여되나요?**</span><span class="sxs-lookup"><span data-stu-id="b1d62-138">**403 Forbidden: Does the user have access and are they licensed?**</span></span>

<span data-ttu-id="b1d62-139">위임된 코드 흐름의 경우 Microsoft Graph는 앱에 부여된 권한과 로그인한 사용자가 가진 권한을 기준으로 요청이 허용되었는지 여부를 평가합니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-139">For delegated code flows, Microsoft Graph evaluates whether the request has been allowed based on the permissions granted to the app and the permissions that the signed-in user has.</span></span> <span data-ttu-id="b1d62-140">일반적으로 이 오류는 사용자가 요청을 수행할 수 있는 권한이 없는 경우 **또는** 액세스 중인 데이터에 대한 라이센스가 없음을 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-140">Generally, this error indicates that the user is not privileged enough to perform the request **or** the user is not licensed for the data being accessed.</span></span> <span data-ttu-id="b1d62-141">필요한 권한 또는 라이선스를 가진 사용자만 성공적으로 요청을 수행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-141">Only users with the required permissions or licenses can make the request successfully.</span></span>

<span data-ttu-id="b1d62-142">**403 Forbidden: 올바른 리소스 API를 선택했나요?**</span><span class="sxs-lookup"><span data-stu-id="b1d62-142">**403 Forbidden: Did you select the correct resource API?**</span></span>

<span data-ttu-id="b1d62-143">Microsoft Graph와 같은 API 서비스는 수신된 액세스 토큰의 *aud* 클레임(청중)이 스스로 기대하는 값과 일치하는지 확인하고, 그렇지 않으면 403 Forbidden error가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-143">API services like Microsoft Graph check that the *aud* claim (audience) in the received access token matches the value it expects for itself, and if not, a 403 Forbidden error occurs.</span></span> <span data-ttu-id="b1d62-144">이 오류가 발생하는 일반적인 오류는 Azure AD Graph API, Outlook API 또는 SharePoint/OneDrive API에 대해 획득한 토큰을 사용하여 Microsoft Graph를 호출하거나 그 반대입니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-144">A common mistake resulting in this error is trying to use a token acquired for Azure AD Graph APIs, Outlook APIs, or SharePoint/OneDrive APIs to call Microsoft Graph (or vice versa).</span></span> <span data-ttu-id="b1d62-145">앱에서 토큰을 획득하는 리소스(또는 범위)가 앱이 호출하는 API와 일치하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-145">Ensure that the resource (or scope) your app is acquiring a token for matches the API that the app is calling.</span></span>

<span data-ttu-id="b1d62-146">**400 Bad Request or 403 Forbidden: 사용자가 조직의 CA(조건부 액세스) 정책을 준수하나요?**</span><span class="sxs-lookup"><span data-stu-id="b1d62-146">**400 Bad Request or 403 Forbidden: Does the user comply with their organization's conditional access (CA) policies?**</span></span>

<span data-ttu-id="b1d62-147">조직의 CA(조건부 액세스) 정책에 따라 앱을 통해 Microsoft Graph 리소스에 액세스하는 사용자에게 앱이 처음 획득한 액세스 토큰에 없는 추가 정보가 필요할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-147">Based on an organization's conditional access (CA) policies, a user accessing Microsoft Graph resources via your app may be challenged for additional information that is not present in the access token your app originally acquired.</span></span> <span data-ttu-id="b1d62-148">이 경우 액세스 토큰을 획득할 때 **400 *interaction_required*** 오류를 받거나 Microsoft Graph를 호출할 때 **403 *insufficient_claims*** 를 받습니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-148">In this case, your app receives a **400 with an *interaction_required*** error during access token acquisition or a **403 with *insufficient_claims*** error when calling Microsoft Graph.</span></span> <span data-ttu-id="b1d62-149">두 경우 모두 오류 응답에는 사용자에게 다단계 인증 또는 장치 등록과 같은 추가 정보를 요청하기 위해 인증된 끝점에 표시할 수 있는 추가 정보가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-149">In both cases, the error response contains additional information that can be presented to the authorized endpoint to challenge the user for additional information (like multi-factor authentication or device enrollment).</span></span>

<span data-ttu-id="b1d62-150">조건부 액세스와 관련된 자세한 내용은 다음을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b1d62-150">For more information related to conditional access, see:</span></span>

- [<span data-ttu-id="b1d62-151">MSAL을 사용하여 조건부 액세스 문제 처리</span><span class="sxs-lookup"><span data-stu-id="b1d62-151">Handling conditional access challenges using MSAL</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [<span data-ttu-id="b1d62-152">Azure Active Directory 조건부 액세스에 대한 개발자 가이드</span><span class="sxs-lookup"><span data-stu-id="b1d62-152">Developer guidance for Azure Active Directory conditional access</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

<span data-ttu-id="b1d62-153">\**_ADAL(Azure Active Directory 인증 라이브러리) 및 AZure AD 그래프 API(AAD Graph) 지원 종료_* _</span><span class="sxs-lookup"><span data-stu-id="b1d62-153">\**_End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)_* _</span></span>

- <span data-ttu-id="b1d62-154">2020년 6월 30일부터 ADAL(Azure Active Directory 인증 라이브러리) 및 AAD 그래프 API(Azure AD Graph API)에 새로운 기능을 더 이상 추가하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-154">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="b1d62-155">기술 지원 및 보안 업데이트를 계속 제공하지만 기능 업데이트는 더 이상 제공하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-155">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
- <span data-ttu-id="b1d62-156">2022년 6월 30일부터 ADAL 및 AAD Graph에 대한 지원을 종료하고 더 이상 기술 지원이나 보안 업데이트를 제공하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-156">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span>
    - <span data-ttu-id="b1d62-157">기존 OS 버전에서 ADAL을 사용하는 앱은 이 시간 이후에도 계속 작동하지만 기술 지원이나 보안 업데이트를 받지 못합니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-157">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>
    - <span data-ttu-id="b1d62-158">이 시간 이후 AAD 그래프를 사용하는 앱은 더 이상 AAD 그래프 엔드포인트에서 응답을 받지 못할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-158">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint.</span></span>

<span data-ttu-id="b1d62-159">_ *ADAL 마이그레이션*\*</span><span class="sxs-lookup"><span data-stu-id="b1d62-159">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="b1d62-160">최신 기능 및 보안 업데이트가 있는 [MSAL(Microsoft Authentication Library)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)로 업데이트하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-160">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span> <span data-ttu-id="b1d62-161">이 권장 사항은 Microsoft가 지원 종료 시한까지 응용 프로그램을 MSAL로 마이그레이션하는 경우에 해당합니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-161">This recommendation is in the context of Microsoft migrating its applications to MSAL by the end-of-support deadline.</span></span> <span data-ttu-id="b1d62-162">Microsoft 앱을 MSAL로 마이그레이션하는 목적은 앱이 MSAL의 지속적인 보안 및 기능 향상의 혜택을 받기 위한 것입니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-162">The objective of Microsoft apps' migration to MSAL is to ensure that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

- [<span data-ttu-id="b1d62-163">ADAL FAQ 읽기</span><span class="sxs-lookup"><span data-stu-id="b1d62-163">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [<span data-ttu-id="b1d62-164">플랫폼별로 앱을 마이그레이션하는 방법 알아보기</span><span class="sxs-lookup"><span data-stu-id="b1d62-164">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- <span data-ttu-id="b1d62-165">ADAL을 사용하는 앱을 이해하는 데 도움이 필요한 경우 모든 앱의 소스 코드를 검토하고 해당하는 경우 ISV(독립 소프트웨어 벤더) 또는 앱 공급자에게 문의하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-165">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="b1d62-166">또한 Microsoft 지원을 통해 테넌트에 있는 Microsoft가 아닌 모든 ADAL 앱 목록을 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-166">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="b1d62-167">**AAD 그래프 마이그레이션**</span><span class="sxs-lookup"><span data-stu-id="b1d62-167">**AAD Graph Migration**</span></span>

<span data-ttu-id="b1d62-168">AAD 그래프를 사용하는 응용 프로그램의 경우 다음 지침에 따라 [Azure AD Graph 응용 프로그램을 Microsoft Graph로 마이그레이션](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true)하세요.</span><span class="sxs-lookup"><span data-stu-id="b1d62-168">For applications that are using AAD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).</span></span>

- <span data-ttu-id="b1d62-169">[마이그레이션 점검표를 통해 시작 지점 제공](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)</span><span class="sxs-lookup"><span data-stu-id="b1d62-169">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
- <span data-ttu-id="b1d62-170">Azure 앱 등록 포털에 AAD 그래프를 사용하는 응용 프로그램이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-170">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="b1d62-171">모든 앱의 소스 코드를 검토하고 해당되는 경우 ISV 또는 앱 공급자에게 문의하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-171">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="b1d62-172">또한 Microsoft 지원은 테넌트의 모든 AAD 그래프 사용에 대한 정보를 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b1d62-172">Microsoft support can also provide you the information of all AAD Graph usage in your tenant.</span></span>

 










