---
title: 원활한 SSO를 내 On-프레미스 앱과 통합할 때의 문제
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
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49848775"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>원활한 SSO를 내 On-프레미스 앱과 통합할 때의 문제

원활한 SSO와 원활한 SSO를 통합하는 문제를 해결하기 위해 다음을 실행합니다.

**권장 단계**

1. 응용 프로그램  프록시를 통한 Single **Sign-On에** 대한 On-프레미스 응용 프로그램을 구성하는 경우 응용 프로그램 프록시를 사용하는 Single Sign-On에 대한 암호 자격 증명 [모음을 참조하세요.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
1. **응용 프로그램** 프록시 문제 해결 : 응용 프로그램 프록시 커넥터가 올바르게 구성되어 있는지 확인하려면 문제 해결 흐름, 응용 프로그램 프록시 커넥터 디버그 문제를 검토하는 것이 좋습니다. [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors) 응용 프로그램에 연결하는 데 여전히 문제가 있는 경우 응용 프로그램 프록시 응용 프로그램 디버그 문제의 문제 해결 [단계를 따릅니다.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) 다음 브라우저 [디버그](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) 도구를 사용하여 CORS 문제를 식별할 수 있습니다.
    1. 브라우저를 시작하고 웹 앱으로 탐색합니다.
    1. **F12를 눌러** 디버그 콘솔을 니다.
    1. 트랜잭션을 재현하고 콘솔 메시지를 검토합니다. CORS 위반으로 원점에 대한 콘솔 오류가 발생합니다.
    1. 앱이 인증을 위해 인증을 위해 login.microsoftonline.com 때 액세스 토큰이 만료되는 경우와 같은 일부 CORS 문제를 해결할 수 없습니다. 그러면 CORS 호출이 실패합니다. 이 시나리오의 해결 해결은 액세스 토큰의 수명을 연장하여 사용자 세션 중 만료되지 않도록 하는 것입니다. 이 작업을 하는 방법에 대한 자세한 내용은 Microsoft ID 플랫폼에서 구성 가능한 토큰 [수명을 참조하세요.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)

**추천 문서**

- [응용 프로그램 프록시 응용 프로그램에 대한 Single Sign-On을 구성하는 방법](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [응용 프로그램 프록시를 사용하는 On-프레미스 응용 프로그램에 대한 SAML Single Sign-On](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Azure Active Directory 응용 프로그램 프록시 CORS 문제 이해 및 해결](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [응용 프로그램 프록시에 대한 Kerberos 제한 위임 구성 문제 해결](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)