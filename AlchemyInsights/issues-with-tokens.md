---
title: 토큰 문제
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7774"
- "9004351"
ms.openlocfilehash: a4e99f1f80df601ddf53498d9a8323790fc52a50b2e067f17429da0bf6a03c43
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067450"
---
# <a name="issues-with-tokens"></a>토큰 문제

토큰과 관련된 문제를 관리하려면 다음 단계를 수행합니다.

1. Microsoft ID 플랫폼에서 발급한 액세스, ID 또는 SAML 토큰의 수명을 지정할 수 있습니다. 조직의 모든 앱, 다중 테넌트(여러 조직) 응용 프로그램 또는 조직의 특정 서비스 주체에 대해 토큰 수명을 설정할 수 있습니다. 자세한 내용은 [Microsoft ID 플랫폼에서 구성 가능한 토큰 수명(미리 보기)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)을 참조하세요.
2. 액세스 토큰을 사용하면 클라이언트가 보호된 웹 API를 안전하게 호출할 수 있으며, 웹 API에서 인증 및 인증을 수행하는 데 사용됩니다. OAuth 설정에 따라 액세스 토큰은 설정된 형식이 없는 불투명 문자열입니다. IDP(ID 제공자)는 GUID를 사용하고, 다른 IDP는 암호화된 blob을 사용합니다. Microsoft ID 플랫폼은 토큰을 받아들이는 API의 구성에 따라 다양한 액세스 토큰 형식을 사용합니다. API에서 액세스 토큰 내부 클레임의 유효성을 검사하고 사용하는 방법을 알아보려면 [Microsoft ID 플랫폼 액세스 토큰](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint)을 참조하세요.
3. MSAL(Microsoft 라이브러리)은 여러 응용 프로그램 시나리오에서 사용할 수 있도록 여러 인증 흐름을 지원합니다. 자세한 내용은 [인증 흐름](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes)을 참조하세요.
4. OAuth 2.0 인증 코드 부여는 장치에 설치된 앱에서 웹 API와 같은 보호된 리소스에 액세스할 수 있습니다. OAuth 2.0의 Microsoft ID 플랫폼 구현을 사용하여 모바일 및 데스크톱 앱에 로그인 및 API 액세스를 추가할 수 있습니다. 모든 언어를 사용하여 응용 프로그램의 프로토콜에 대해 직접 프로그래밍하는 방법은 [Microsoft ID 플랫폼 및 OAuth 2.0 인증 코드 흐름](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token)을 참조하세요.
5. OIDC(OpenID Connect)는 OAuth 2.0을 기반으로 구축된 인증 프로토콜로, 사용자를 응용 프로그램에 안전하게 서명하는 데 사용할 수 있습니다. Microsoft ID 플랫폼 끝점의 OpenID Connect 구현을 사용하면 앱에 로그인 및 API 액세스를 추가할 수 있습니다. [Microsoft ID 플랫폼 및 OpenID Connect 프로토콜](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request)은 언어와 무관하게 이 작업을 수행하는 방법을 보여주며 Microsoft 오픈 소스 라이브러리를 사용하지 않고 HTTP 메시지를 보내고 받는 방법을 설명합니다.
    - UserInfo 끝점은 인증된 사용자에 대한 클레임을 반환하도록 설계된 OIDC 표준의 일부입니다. 자세한 내용은 [Microsoft ID 플랫폼 UserInfo 끝점](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead)을 참조하세요.
    - [Azure AD 및 OpenID Connect를 사용하여 웹앱에서 웹 API 호출](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) 샘플은 OpenID Connect를 사용하여 Azure AD를 로그인하기 위해 MVC 웹 응용 프로그램을 작성하는 방법을 보여 줍니다. 그런 다음 OAuth 2.0을 통해 얻은 토큰을 사용하여 로그인한 사용자의 ID로 웹 API를 호출합니다. 이 샘플에서는 OpenID Connect ASP .Net OWIN 미들웨어 및 ADAL .Net.을 사용합니다.
6. [웹 API를 표시하도록 응용 프로그램 구성
](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) - 이 빠른 시작에서는 Microsoft ID 플랫폼에 웹 API를 등록하고 예제 범위를 추가하여 클라이언트 앱에 노출합니다. 웹 API를 등록하고 범위를 통해 노출하면 권한 있는 사용자 및 API에 액세스하는 클라이언트 앱에 해당 리소스에 대한 권한 기반 액세스를 제공할 수 있습니다.
7. Azure AD B2C(Azure Active Directory B2C)에서 ROPC(리소스 소유자 암호 자격 증명) 흐름은 OAuth 표준 인증 흐름입니다. 이 흐름에서 신뢰 당사자라고도 하는 응용 프로그램은 토큰과 유효한 자격 증명을 교환합니다. 자격 증명에는 사용자 ID 및 암호가 포함됩니다. 반환되는 토큰은 ID 토큰, 액세스 토큰 및 새로 고침 토큰입니다. 자세한 내용은 [Azure Active Directory B2C에서 리소스 소유자 암호 자격 증명 흐름 설정](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow)을 참조하세요. 

