---
title: 원활한 SSO를 내 사내 앱과 통합하는 데 문제가 있습니다.
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 6b295f3272ba074eac3afb66f3156af7ea4065a1398a215bcb3cde5da74b198a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028298"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>원활한 SSO를 내 사내 앱과 통합하는 데 문제가 있습니다.

Seamless SSO를 사내 응용 프로그램과 통합하는 문제를 해결하기 위해 다음을 실행합니다.

**다음 권장 단계**

1. 응용 프로그램 프록시를 통해 Single **Sign-On에** 대한 **On-프레미스** 응용 프로그램을 구성하기 위해 응용 프로그램 프록시를 사용하는 Single Sign-On에 대한 암호 자격 증명 [모음을 참조하세요.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
1. **응용 프로그램** 프록시 문제 해결 : 문제 해결 흐름, [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)응용 프로그램 프록시 커넥터 디버그 문제부터 검토하여 응용 프로그램 프록시 커넥터가 올바르게 구성되어 있는지 확인하는 것이 좋습니다. 여전히 응용 프로그램에 연결하는 데 문제가 있는 경우 [응용 프로그램 프록시 문제 버그](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)의 문제 해결 단계를 따르세요. 다음 브라우저 디버그 도구를 사용하여 [CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) 문제를 식별할 수 있습니다.
    1. 브라우저를 실행하고 웹앱으로 이동합니다.
    1. **F12** 를 눌러 디버그 콘솔을 불러옵니다.
    1. 트랜잭션을 재현하고 콘솔 메시지를 검토합니다. CORS 위반은 원본에 대한 콘솔 오류를 생성합니다.
    1. 일부 CORS 문제는 앱이 인증을 위해 login.microsoftonline.com 때와 액세스 토큰이 만료되는 경우와 같이 해결할 수 없습니다. 그러면 CORS 호출이 실패합니다. 이 시나리오의 해결 방법은 사용자 세션 중에 액세스 토큰이 만료되지 않도록 액세스 토큰의 수명을 연장하는 것입니다. 이 문제를 해결하는 방법에 대한 자세한 내용은 [Microsoft ID 플랫폼에서 구성 가능한 토큰 수명](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)을 참조하세요.

**추천 문서**

- [응용 프로그램 프록시 응용 프로그램에 대한 Single Sign-On을 구성하는 방법](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [응용 프로그램 프록시를 사용하는 사내 응용 프로그램에 대한 SAML Single Sign-On](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [응용 프로그램 프록시 CORS Azure Active Directory 이해 및 해결](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [응용 프로그램 프록시에 대한 Kerberos 제한된 위임 구성 문제 해결](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)