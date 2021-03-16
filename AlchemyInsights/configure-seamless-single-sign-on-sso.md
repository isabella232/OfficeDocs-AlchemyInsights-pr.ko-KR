---
title: 원활한 SSO(Single Sign-On) 구성
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
- "9004344"
- "9384"
ms.openlocfilehash: 32790b23547de36cd2864e85ebae67f54ad91707
ms.sourcegitcommit: 309b9f3e6e2ff622f95bb860d337d2c05b7bbe54
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/15/2021
ms.locfileid: "50819570"
---
# <a name="configure-seamless-single-sign-on-sso"></a>원활한 SSO(Single Sign-On) 구성

**응용 프로그램 구성**

1. 응용 프로그램 공급업체로부터 값을 얻게 됩니다. 값을 수동으로 입력하거나 메타데이터 파일을 업로드하여 필드 값을 추출할 수 있습니다.
2. 많은 앱이 Azure AD에서 작동하도록 이미 미리 구성되어 있습니다. 이러한 앱은 Azure AD 테넌트에 앱을 추가할 때 찾아볼 수 있는 앱 갤러리에 나열됩니다. 빠른 [시작 시리즈는](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) 프로세스를 진행합니다.
3. 갤러리가 아닌 응용 프로그램을 만들려면 **+** 자체 응용 프로그램 만들기 단추를 클릭하고 응용 프로그램에 이름을 지정합니다.
    - 기본적으로 갤러리에서 찾을  수 없는 다른 응용 프로그램 통합(갤러리가 아닌 응용 프로그램에 대한 올바른 옵션)을 선택합니다.
    - 응용 프로그램의 이름을 입력한 후 **Create를** 실행하면 갤러리가 아닌 새 엔터프라이즈 응용 프로그램이 생성됩니다.
    - 그런 다음 해당 응용 프로그램 관리에서 **Single Sign-On으로** 이동하면 해당 환경에서 구현하기 위한 다양한 기술을 볼 수 있습니다. 

**특정 응용 프로그램에 대해 Seamless SSO 구성**

갤러리의 앱에 대한 자세한 단계별 지침이 있습니다. 단계에 액세스하려면 SaaS 앱 구성 자습서 에서 모든 앱 구성 자습서 목록을 [찾아볼 수 있습니다.](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)

**SAML 기반 SSO 구성**

1. 빠른 시작: Azure AD(Azure Active Directory) 테넌트의 응용 프로그램에 대해 SAML 기반 [SSO(Single Sign-On)를 설치합니다.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)
2. Single Sign-On에 대한 SAML 기반 옵션에 대한 자세한 내용은 SAML 기반 Single Sign-On 이해를 [참조하세요.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)
3. Azure AD(Azure Active Directory)가 SSO(Single Sign-On)에 대해 지원하는 SAML 2.0 인증 요청 및 응답에 대한 자세한 내용은 Single Sign-On [SAML 프로토콜을 참조하세요.](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
4. Microsoft Graph API를 사용하여 Azure AD(Azure Active Directory)에서 응용 프로그램에 대한 SAML 기반 SSO(Single Sign-On)를 만들고 구성하는 방법에 대한 자세한 내용은 Microsoft Graph API를 사용하여 응용 프로그램에 대한 SAML 기반 Single [Sign-On 구성을](https://docs.microsoft.com/graph/application-saml-sso-configure-api)참조하세요.
5. Azure AD에서 SAML 프로토콜을 사용하는 방법에 대한 자세한 내용은 Microsoft ID 플랫폼에서 SAML 프로토콜을 사용하는 [방법을 참조하세요.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference)

**토큰 및 클레임 구성**

1. 방법: 엔터프라이즈 응용 프로그램의 SAML 토큰에서 [발급된 클레임 사용자 지정](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)
2. PowerShell을 사용하여 클레임 구성 방법에 대한 자세한 내용은 방법: 테넌트의 특정 앱에 대해 토큰으로 내보인 클레임 사용자 [지정(미리 보기)을 참조하세요.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
3. 선택적 클레임 구성 방법에 대한 자세한 내용은 방법: 앱에 선택적 클레임 [제공을 참조하세요.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
4. 토큰 클레임의 응용 프로그램으로 사용자 데이터를 보내는 데 디렉터리 Schema 확장 특성을 사용하는 방법에 대한 자세한 내용은 클레임에서 디렉터리 [schema 확장 특성 사용을 참조합니다.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions)
5. 토큰 수명을 구성하는 방법에 대한 자세한 내용은 Microsoft ID 플랫폼(미리 보기)에서 구성 가능한 토큰 [수명을 참조합니다.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
6. [토큰 수명 정책 구성(미리 보기)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) - 이 문서에서는 토큰 수명에 대한 새 규칙을 적용하는 데 도움이 되는 일반적인 정책 시나리오를 설명합니다. 이 예제에서는 사용자가 웹 앱에서 더 자주 인증해야 하는 정책을 만드는 방법을 배웠습니다.

**SSO 구성 문제 해결**

- Azure Active Directory Seamless SSO(Seamless Single Sign-On)에 대한 질문과 대답은 [Azure Active Directory Seamless Single Sign-On: 질문과](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq)대답을 참조하세요.
- Azure AD(Azure Active Directory) Seamless SSO(Seamless Single Sign-On)에 관한 일반적인 문제에 대한 문제 해결 정보는 Azure Active Directory 원활한 Single Sign-On 문제 해결을 [참조하세요.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)
