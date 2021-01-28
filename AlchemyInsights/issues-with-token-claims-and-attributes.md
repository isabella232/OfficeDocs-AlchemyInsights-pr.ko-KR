---
title: 토큰 클레임 및 특성 관련 문제
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
- "9004347"
- "7761"
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50029989"
---
# <a name="issues-with-token-claims-and-attributes"></a><span data-ttu-id="cf48d-102">토큰 클레임 및 특성 관련 문제</span><span class="sxs-lookup"><span data-stu-id="cf48d-102">Issues with Token Claims and Attributes</span></span>

<span data-ttu-id="cf48d-103">**토큰 클레임 업데이트, 구성 또는 제거**</span><span class="sxs-lookup"><span data-stu-id="cf48d-103">**Update, configure or remove token claims**</span></span>

1. <span data-ttu-id="cf48d-104">Azure AD(Azure Active Directory)를 사용하면 앱에 권한을 승인한 후 받은 응답 토큰에서 역할 클레임에 대한 클레임 유형을 사용자 지정할 수 있습니다. [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management)</span><span class="sxs-lookup"><span data-stu-id="cf48d-104">By using Azure Active Directory (Azure AD), you can [customize the claim type for the role claim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) in the response token that you receive after you authorize an app.</span></span>
2. <span data-ttu-id="cf48d-105">응용 프로그램 개발자는 Azure AD 응용 프로그램에서 선택적 클레임을 사용하여 응용 프로그램으로 전송되는 토큰에서 원하는 클레임을 지정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cf48d-105">Application developers can use optional claims in their Azure AD applications to specify which claims they want in tokens sent to their application.</span></span> <span data-ttu-id="cf48d-106">자세한 내용은 앱에 [대한 선택적 클레임 제공을 참조하세요.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)</span><span class="sxs-lookup"><span data-stu-id="cf48d-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
3. <span data-ttu-id="cf48d-107">Azure Active Directory를 사용하여 응용 프로그램에 [대한 그룹 클레임 구성](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)</span><span class="sxs-lookup"><span data-stu-id="cf48d-107">[Configure group claims for applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span></span>
4. <span data-ttu-id="cf48d-108">응용 프로그램에서 Seamless Single Sign-On을 사용하는 경우 엔터프라이즈 응용 프로그램에 대한 SAML 토큰에서 발급된 클레임 사용자 [지정을 참조합니다.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)</span><span class="sxs-lookup"><span data-stu-id="cf48d-108">If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>

<span data-ttu-id="cf48d-109">**클레임 특성 매핑**</span><span class="sxs-lookup"><span data-stu-id="cf48d-109">**Claims Attribute Mapping**</span></span>

1. <span data-ttu-id="cf48d-110">PowerShell을 사용하여 클레임 매핑 정책을 구성하기 위해 테넌트의 특정 앱에 대한 토큰으로 내보인 클레임 사용자 지정(미리 보기)을 [참조하세요.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)</span><span class="sxs-lookup"><span data-stu-id="cf48d-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
2. <span data-ttu-id="cf48d-111">디렉터리 Schema 확장 특성은 사용자 개체 및 기타 디렉터리 개체(예: 그룹, 테넌트 세부 정보, 서비스 주체)에 Azure Active Directory에 추가 데이터를 저장할 수 있는 방법을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="cf48d-111">Directory schema extension attributes provide a way to store additional data in Azure Active Directory on user objects and other directory objects such as groups, tenant details, service principals.</span></span> <span data-ttu-id="cf48d-112">응용 프로그램에 클레임이 표시될 때 사용자 개체의 확장 특성만 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cf48d-112">Only extension attributes on user objects can be used for emitting claims to applications.</span></span> <span data-ttu-id="cf48d-113">[클레임에서 디렉터리 schema 확장](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) 특성을 사용하여 토큰 클레임의 응용 프로그램으로 사용자 데이터를 전송하는 데 디렉터리 schema 확장 특성을 사용하는 방법을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="cf48d-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span></span>

<span data-ttu-id="cf48d-114">토큰 클레임에 대한 자세한 내용은 다음을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cf48d-114">For more information on token claims, see:</span></span>

- [<span data-ttu-id="cf48d-115">액세스 토큰의 클레임</span><span class="sxs-lookup"><span data-stu-id="cf48d-115">Claims in access tokens</span></span>](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [<span data-ttu-id="cf48d-116">클레임의 id_token</span><span class="sxs-lookup"><span data-stu-id="cf48d-116">Claims in an id_token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- <span data-ttu-id="cf48d-117">[](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) Azure AD B2C에서 발급한 ID 토큰 및 액세스 토큰에서 기대할 수 있는 클레임</span><span class="sxs-lookup"><span data-stu-id="cf48d-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span></span>
- [<span data-ttu-id="cf48d-118">SAML 토큰 클레임 참조</span><span class="sxs-lookup"><span data-stu-id="cf48d-118">SAML token claims reference</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
