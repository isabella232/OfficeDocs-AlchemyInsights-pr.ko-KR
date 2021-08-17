---
title: SSO 연결 문제
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
- "9004357"
- "7810"
ms.openlocfilehash: 8fb93bc40c6cd5a7c0e3d259fe3be8d1bab3187dd5aa023eb49977555fd930de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084352"
---
# <a name="sso-connection-issues"></a>SSO 연결 문제

1. 응용 프로그램을 구성하려면 [빠른 시작: 응용 프로그램 속성 구성](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) 가이드를 따르세요.
2. 선택한 응용 프로그램 및 [Single Sign-On](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) 옵션에 따라 아래 적절한 지침을 따르세요.
    - SAML  기반 Single **Sign-On에** 대한 사내 응용 프로그램을 구성하는 경우 응용 프로그램 프록시를 사용하여 사내 응용 프로그램에 대한 [SAML Single Sign-On을 참조합니다.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
    - 암호 기반  Single **Sign-On에** 대한 클라우드 응용 프로그램을 구성하는 경우 [암호 Single Sign-On 구성을 참조하세요.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)
    - 응용 프로그램 프록시를 통해 Single **Sign-On에** 대한 **On-프레미스** 응용 프로그램을 구성하기 위해 응용 프로그램 프록시를 사용하는 Single Sign-On에 대한 암호 자격 증명 [모음을 참조하세요.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
3. 응용 프로그램 프록시 문제 **해결:** 문제 해결 흐름, [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)응용 프로그램 프록시 커넥터 디버그 문제부터 검토하여 응용 프로그램 프록시 커넥터가 올바르게 구성되어 있는지 확인하는 것이 좋습니다. 응용 프로그램에 연결하는 데 여전히 문제가 있는 경우 응용 프로그램 프록시 응용 프로그램 디버그 문제 의 문제 [해결 흐름을 따르는 것이 좋습니다.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) 브라우저 [디버그](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) 도구를 사용하여 CORS 문제를 식별할 수 있습니다.
    - 브라우저를 실행하고 웹앱으로 이동합니다.
    - **F12** 를 눌러 디버그 콘솔을 불러옵니다.
    - 트랜잭션을 재현하고 콘솔 메시지를 검토합니다. CORS 위반은 원본에 대한 콘솔 오류를 생성합니다.
    - 일부 CORS 문제는 앱이 인증을 위해 인증을 위해 login.microsoft.com 때와 같은 문제를 해결할 수 없습니다. 그러면 CORS 호출이 실패합니다. 이 시나리오의 해결 방법은 사용자 세션 중에 액세스 토큰이 만료되지 않도록 액세스 토큰의 수명을 연장하는 것입니다. 이 문제를 해결하는 방법에 대한 자세한 내용은 [Microsoft ID 플랫폼에서 구성 가능한 토큰 수명](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)을 참조하세요.
4. SAML 기반 Single **Sign-On** 문제 해결 : SAML 기반 Single [Sign-On](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)구성된 앱에 로그인하는 문제를 확인하여 발생할 가능성이 높은 문제에 대한 해결 방법을 찾는 것이 좋습니다.
5. 암호 기반 Single **Sign-On** 문제 해결 : Azure AD에서 암호 기반 Single [Sign-On](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)문제 해결을 확인하여 발생할 가능성이 높은 문제에 대한 해결 방법을 찾는 것이 좋습니다.
6. VPN을 사용하는 동안 연결 문제에 대한 자세한 내용은 VPN을 통해 [SSO(Single Sign On)를](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)사용하는 방법 및 연결 Wi-Fi 참조하세요.
