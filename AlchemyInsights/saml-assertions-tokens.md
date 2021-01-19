---
title: SAML Assertions(토큰)
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
- "9004341"
- "7753"
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884617"
---
# <a name="saml-assertions-tokens"></a><span data-ttu-id="ee10c-102">SAML Assertions(토큰)</span><span class="sxs-lookup"><span data-stu-id="ee10c-102">SAML Assertions (Tokens)</span></span>

1. <span data-ttu-id="ee10c-103">SAML(Security Assertions Markup Language) 토큰은 클레임의 XML 표현입니다.</span><span class="sxs-lookup"><span data-stu-id="ee10c-103">Security Assertions Markup Language (SAML) tokens are XML representations of claims.</span></span> <span data-ttu-id="ee10c-104">기본적으로 페더임된 보안 시나리오에서 WCF(Windows Communication Foundation)에서 사용하는 SAML 토큰은 토큰을 발급합니다.</span><span class="sxs-lookup"><span data-stu-id="ee10c-104">By default, SAML tokens Windows Communication Foundation (WCF) uses in federated security scenarios are issued tokens.</span></span> <span data-ttu-id="ee10c-105">자세한 내용은 SAML 토큰 및 [클레임 을 참조하세요.](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims)</span><span class="sxs-lookup"><span data-stu-id="ee10c-105">For more information, see [SAML Tokens and Claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span></span>
2. <span data-ttu-id="ee10c-106">Microsoft ID 플랫폼은 각 인증 흐름의 처리에서 여러 유형의 보안 토큰을 내보냅니다.</span><span class="sxs-lookup"><span data-stu-id="ee10c-106">The Microsoft identity platform emits several types of security tokens in the processing of each authentication flow.</span></span> <span data-ttu-id="ee10c-107">[SAML 토큰 클레임 참조는](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) SAML 2.0 토큰의 형식, 보안 특성 및 콘텐츠를 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="ee10c-107">[SAML token claims reference](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) describes the format, security characteristics, and contents of SAML 2.0 tokens.</span></span>
3. <span data-ttu-id="ee10c-108">Microsoft ID 플랫폼의 구성 [가능한](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) 토큰 수명에 대한 지침에 따라 토큰 수명을 구성하는 방법을 이해합니다.</span><span class="sxs-lookup"><span data-stu-id="ee10c-108">Follow the guidance in [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) to understand how to configure token lifetimes.</span></span>
4. <span data-ttu-id="ee10c-109">이 문서에 설명된 단계에 따라 Azure AD SAML 토큰 암호화를 구성하는 방법을 이해합니다. [](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption)</span><span class="sxs-lookup"><span data-stu-id="ee10c-109">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) to understand how to configure Azure AD SAML token encryption.</span></span>
5. <span data-ttu-id="ee10c-110">Azure AD에서 인증서 서명 옵션 및 인증서 서명 알고리즘을 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ee10c-110">In Azure AD, you can set up certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="ee10c-111">자세한 내용은 Azure Active Directory의 갤러리 앱에 대한 SAML 토큰의 고급 인증서 서명 [옵션을 참조하세요.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)</span><span class="sxs-lookup"><span data-stu-id="ee10c-111">For more information, see [Advanced certificate signing options in the SAML token for gallery apps in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>
