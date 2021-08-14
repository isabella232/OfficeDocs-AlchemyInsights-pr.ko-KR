---
title: SSO 구성 문제
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7760"
- "9004346"
ms.openlocfilehash: c843e9315776f3dbab2f25c864ebe8b0c41000b8ce70046fe4eb386fce143635
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54009578"
---
# <a name="sso-configuration-issues"></a>SSO 구성 문제

1. 응용 프로그램을 구성하려면 [빠른 시작: 응용 프로그램 속성 구성](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) 가이드를 따르세요.
2. 선택한 응용프로그램 및 [Single Sign-On 옵션](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options)에 따라 아래의 해당 지침을 따르세요. a. **SAML 기반 SSO(Single Sign-On)** 에 대해 **온-프레미스 응용 프로그램** 을 구성하려면 [응용 프로그램 프록시를 사용하는 온-프레미스 응용 프로그램의 SAML Single Sign-On](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)을 참조하세요.
    b. **암호 기반 SSO** 에 대해 **클라우드 응용 프로그램** 을 구성하려면 [암호 Single Sign-On 구성](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)을 참조하세요.
    c. **SSO를 통한 응용 프로그램 프록시** 에 대해 **온-프레미스 응용 프로그램** 을 구성하려면 [응용 프로그램 프록시를 사용한 Single Sign-On용 암호 재설정](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)을 참조하세요.
3. **응용 프로그램 프록시 문제 해결**: 먼저 문제 해결 흐름의 [응용 프로그램 프록시 커넥터 문제 디버그](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)를 검토하여 응용 프로그램 프록시 커넥터가 올바르게 구성되어 있는지 확인하는 것이 좋습니다. 여전히 응용 프로그램에 연결하는 데 문제가 있는 경우 [응용 프로그램 프록시 문제 버그](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)의 문제 해결 단계를 따르세요. 다음 브라우저 디버그 단계를 수행하여 [CORS 문제 식별](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues)할 수 있습니다. a. 브라우저를 실행하고 웹앱으로 이동합니다.
    b. **F12** 를 눌러 디버그 콘솔을 불러옵니다.
    c. 트랜잭션을 재현하고 콘솔 메시지를 검토합니다. CORS 위반은 원본에 대한 콘솔 오류를 생성합니다.
    d. 앱이 인증을 위해 login.microsoftonline.com으로 리디렉션할 때 액세스 토큰이 만료되는 등의 일부 CORS 문제는 해결할 수 없습니다. 액세스 토큰 만료로 인해 CORS 호출이 실패합니다. 이 시나리오의 해결 방법은 사용자 세션 중에 액세스 토큰이 만료되지 않도록 액세스 토큰의 수명을 연장하는 것입니다. 이 문제를 해결하는 방법에 대한 자세한 내용은 [Microsoft ID 플랫폼에서 구성 가능한 토큰 수명](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)을 참조하세요.
4. **SAML 기반 SSO문제 해결**: 발생할 가능성이 큰 문제에 대한 해결 방법은 [SAML 기반 Single Sign-On 구성된 앱에 문제 해결](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)을 확인하는 것이 좋습니다.
5. **암호 기반 SSO 문제 해결**: Azure AD [ 발생할 가능성이 큰 문제에 대한 해결 방법을 찾으려면](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)Azure AD에서 암호 기반 Single Sign-On 문제 해결을 확인하는 것이 좋습니다.
6. **구성 오류를 받았습니다.** 구성 오류를 해결하려면 다음 문서를 확인하는 것이 좋습니다. a. [SAML 기반 Single Sign-On 구성 앱에 로그인하는 데 문제가 있습니다.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) [자격 증명이 입력되었지만 확장에서 자격 증명을 제출하지 않습니다.](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso#credentials-are-filled-in-but-the-extension-does-not-submit-them) c. [자격 증명이 입력 및 제출되었지만 페이지에 잘못된 자격 증명이 표시됩니다.](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) d. [사용자가 로그인한 후 앱 페이지에 오류 메시지가 표시됩니다.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
7. **온-프레미스 앱과 완벽한 SSO를 통합하는 데 문제가 있습니다.** 온-프레미스 앱과의 완벽한 SSO 통합과 관련된 문제를 해결하려면 다음 문서를 확인하는 것이 좋습니다. a. [응용 프로그램 프록시 응용 프로그램에 대한 단일 로그온을 구성하는 방법](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to) b [응용 프로그램 프록시를 사용하여 온-프레미스 응용 프로그램을 위한 SAML Single Sign-On](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps) c. [Azure Active Directory 응용 프로그램 프록시 CORS 문제를 이해하고 해결](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues) [응용 프로그램 프록시에 대한 Kerberos 제한된 위임 구성 문제 해결](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)
8. **클레임을 고치거나 토큰의 수명을 연장해야 합니다. 세션 길이를 변경해야 합니다.** 이를 위해 다음 문서를 확인하는 것이 좋습니다. a. [응용 프로그램에 전송된 SAML 클레임 사용자 정의](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping) b. [claims-aware 앱으로 작업](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-for-claims-aware-applications) c. [Microsoft ID 플랫폼에서 구성 가능한 토큰 수명](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) d. [조건부 액세스를 사용하여 인증 세션 관리 구성](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime) e. [온-프레미스 응용 프로그램에 액세스하기 위한 쿠키 설정](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-cookie-settings)
9. **사용자 및 게스트 사용자(B2B) 액세스를 관리하는 데 도움이 필요합니다.** 사용자 및 게스트 사용자의 액세스 관리에 대한 자세한 내용은 다음 문서를 확인하는 것이 좋습니다. a. [앱에 대한 액세스 관리](https://docs.microsoft.com/azure/active-directory/manage-apps/what-is-access-management) b. [Azure Active Directory의 앱에 대한 사용자 할당 관리](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal) c. [B2B 공동 작업을 위해 SaaS 앱 구성](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps) d. [Azure AD의 B2B 사용자에게 온-프레미스 응용 프로그램에 대한 액세스 권한 부여](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps) e. [Azure ADB2B 공동 작업을 통해 로컬 관리 파트너 계정에 클라우드 리소스에 대한 액세스 권한 부여](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)
10. **앱을 사용자 지정하고 싶습니다.** 앱 사용자 지정에 대한 자세한 내용은 다음 문서를 확인하는 것이 좋습니다. a. [Azure AD 응용 프로그램 프록시로 사용자 지정 도메인 구성](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-custom-domain) b. [게시된 응용 프로그램의 사용자 지정 홈페이지 설정](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-custom-home-page) c. [와일드카드 응용 프로그램](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-wildcard)
11. **앱을 ADFS에서 Azure로 마이그레이션하는 데 문제가 있습니다.**: 앱을 ADS에서 Azure로 마이그레이션하는 동안 발생한 문제를 해결하려면 다음 문서를 확인하는 것이 좋습니다. a. [](https://docs.microsoft.com/azure/active-directory/manage-apps/migrate-adfs-apps-to-azure) b. [Azure Active Directory로 응용 프로그램 마이그레이션하기 위한 리소스](https://docs.microsoft.com/azure/active-directory/manage-apps/migration-resources)

