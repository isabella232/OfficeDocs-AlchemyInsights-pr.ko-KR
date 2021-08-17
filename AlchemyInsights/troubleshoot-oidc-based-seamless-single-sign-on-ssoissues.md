---
title: OIDC 기반 원활한 SSO(Single Sign-On) 문제 해결
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9375"
ms.openlocfilehash: 5880ee37a2fcc98b34231cc9960fb3f87fa184b07bd81ccd37d0ea5a78170af0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105784"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>OIDC 기반 원활한 SSO(Single Sign-On) 문제 해결

- Azure 테넌트에 OIDC 기반 앱을 추가하는 방법에 대한 자세한 내용은 빠른 시작: Azure AD(Azure AD) 테넌트의 응용 프로그램에 대한 [OIDC 기반 SSO(single sign-on) Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)참조하세요.
- Single Sign-On을 구현하기 위해 OpenID 커넥트 앱에 대한 자세한 내용은 OIDC 기반 Single Sign-On 이해를 [참조하세요.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on)
- 오픈 소스 라이브러리 중 하나를 사용하는 대신 HTTP 요청을 직접 보내고 처리하거나 타사 오픈 소스 라이브러리를 사용하여 코드를 작성하도록 선택하는 경우 의 [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)및 OpenID 커넥트 프로토콜을 Microsoft ID 플랫폼.

**프로토콜**

1. [Microsoft ID 플랫폼](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) 및 암시적 부여 흐름 - 암시적 부여의 정의 특성은 /token 끝점이 아닌 /authorize 끝점에서 직접 /authorize 끝점에서 토큰(ID 토큰 또는 액세스 토큰)을 반환하는 것입니다. 인증 코드와 함께 /authorize 요청에서 ID 토큰을 검색하는 **"하이브리드 흐름"이라는** 권한 부여 코드 흐름의 일부로 자주 사용됩니다. 이 문서에서는 Azure AD에서 토큰을 요청하기 위해 응용 프로그램의 프로토콜에 대해 직접 프로그래밍하는 방법을 설명합니다.
2. [Microsoft ID 플랫폼 및 OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 권한 부여 코드 흐름 - OAuth 2.0 권한 부여 코드 부여는 웹 API와 같은 보호된 리소스에 액세스하기 위해 장치에 설치된 앱에서 사용할 수 있습니다. OAuth 2.0의 Microsoft ID 플랫폼 구현을 사용하여 모바일 및 데스크톱 앱에 로그인 및 API 액세스를 **추가할 수 있습니다.** 이 문서에서는 모든 언어를 사용하여 응용 프로그램의 프로토콜에 대해 직접 프로그래밍하는 방법에 대해 설명합니다.
3. [Microsoft ID 플랫폼 및 OpenID](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) 커넥트 프로토콜 - OpenID Microsoft ID 플랫폼 구현을 사용하는 경우 커넥트 앱에 로그인 및 API 액세스를 추가할 수 있습니다. 이 문서에서는 언어와는 독립적으로 이 작업을 하는 방법을 보여 주며, Microsoft 오픈 소스 라이브러리를 사용하지 않고 HTTP 메시지를 보내고 받는 방법에 **대해 설명하고 있습니다.**
4. [Microsoft ID 플랫폼 및 OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 클라이언트 자격 증명 흐름 - RFC 6749에 지정된 OAuth 2.0 클라이언트 자격 증명을 사용하여 응용 프로그램의 ID를 사용하여 웹 호스트 리소스에 액세스할 수 있습니다. 이러한 유형의 부여는 사용자와의 즉각적인 상호 작용 없이 백그라운드에서 실행해야 하는 서버 간 상호 작용에 일반적으로 사용됩니다. 이러한 유형의 응용 프로그램을 데몬  또는 서비스 **계정이라고도 합니다.** 이 문서에서는 응용 프로그램의 프로토콜에 대해 직접 프로그래밍하는 방법을 설명합니다.
