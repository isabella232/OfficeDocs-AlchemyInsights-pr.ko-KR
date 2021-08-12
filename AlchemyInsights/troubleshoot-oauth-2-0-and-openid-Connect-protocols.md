---
title: OAuth 2.0 및 OpenID Connect 프로토콜 문제 해결
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9776"
- "9004342"
ms.openlocfilehash: 7584d8f6f2e24812c1fdded76332edc6dd671034011e262c15756567cb467c26
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53921049"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>OAuth 2.0 및 OpenID Connect 프로토콜 문제 해결

OAuth 2.0 및 OpenID Connect 문제를 해결하려면 다음 권장 단계를 수행합니다.

OAuth 2.0 및 OpenID Connect 프로토콜 구성 및 문제 해결과 관련된 다음 문서를 참조합니다.

- [Microsoft ID 플랫폼 및 OAuth 2.0 인증 코드 흐름](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) - 이 문서는 여러 언어를 사용하여 응용 프로그램에 **코드 인증(PKCE) 흐름** 을 직접 프로그래밍하는 방법에 관해 설명합니다.
- [Microsoft ID 플랫폼 및 OAuth 2.0 클라이언트 자격 증명 흐름](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) - 이 문서는 여러 언어를 사용하여 응용 프로그램에 **클라이언트 자격 증명 흐름** 을 직접 프로그래밍하는 방법에 관해 설명합니다.
- [Microsoft ID 플랫폼 및 OAuth 2.0 리소스 소유자 암호 자격 증명](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) - 이 문서는 응용 프로그램에 대해 **ROPC 흐름** 을 직접 프로그래밍하는 방법에 관해 설명합니다.
    - Microsoft ID 플랫폼은 개인 계정이 아니라 Azure AD 테넌트용 ROPC만 지원합니다. 즉, 특정 테넌트 끝점 **(https://login.microsoftonline.com/{TenantId_or_Name})** 또는 **조직** 끝점을 사용하야 합니다.
    - Azure AD 테넌트에 초대된 개인 계정은 ROPC를 사용할 수 없습니다.
    - 암호가 없는 계정은 ROPC를 통해 로그인할 수 없습니다. 이 시나리오에서는 앱에 대해 다른 흐름을 사용하는 것이 좋습니다.
    - 사용자가 [MFA(다단계 인증)](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks)을 사용하여 응용 프로그램에 로그인해야 하는 경우, 차단됩니다.
    - ROPC는 [하이브리드 ID 페더레이션](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) 시나리오(예: 온-프레미스 계정을 인증하는 데 사용되는 Microsoft Azure AD 및 ADFS)에서는 지원되지 않습니다. 사용자가 전체 페이지를 온-프레미스 ID 공급자로 리디렉션된 경우 Azure AD는 해당 ID 공급자에 대해 사용자 이름과 암호를 테스트할 수 없습니다. 하지만 [통과 인증](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta)은 ROPC에서 지원됩니다.
    - 하이브리드 ID 페더레이션 시나리오 예외는 다음과 같습니다. **AllowCloudPasswordValidation** 이 **TRUE** 로 설정된 홈 영역 검색 정책을 사용하면 온-프레미스 암호가 클라우드에 동기화될 때 ROPC 흐름이 페더레이션된 사용자에 대해 작동할 수 있습니다. 자세한 내용은 [레거시 응용 프로그램에 관한 페더레이션된 사용자에 대한 직접 ROPC 인증 사용](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications)을 참조하세요. 
- [Microsoft ID 플랫폼 및 OAuth 2.0 On-behalf-Of 흐름](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) - 이 문서는 **OBO(on-behalf-of) 흐름** 에 대해 직접 프로그래밍하는 방법을 설명합니다.
- [Microsoft ID 플랫폼 및 OpenID Connect 프로토콜](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) - 이 문서는 언어와 무관하게 OpenID Connect 프로토콜을 구현하는 방법을 설명하고 Microsoft 오픈 소스 라이브러리를 사용하지 않고 HTTP 메시지를 주고받는 방법에 대해 설명합니다.

**엑세스 토큰**

[Microsoft ID 플랫폼 액세스 토큰](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - API에서 액세스 코튼 내부 클레임의 유효성을 검사하고 사용하는 방법을 알아봅니다. 이 게시물의 모든 문서(설명된 경우를 제외)는 등록한 API에 대해 발급된 토큰에만 적용됩니다. Microsoft 소유 API용으로 발급된 토큰에는 적용되지 않으며 사용자가 생성한 API에 대해 Microsoft ID 플랫폼이 토큰을 발행하는 방법을 확인하는 데 이러한 토큰을 사용할 수도 없습니다.

**응용 프로그램 구성**

[리디렉션 URI(회신 URL) 제한 사항](https://docs.microsoft.com/azure/active-directory/develop/reply-url) - 리디렉션 URI(회신 URL)를 구성하는 방법을 확인합니다. 리디렉션 URI 또는 회신 URL은 앱이 성공적으로 승인되고 권한 코드 또는 액세스 토큰이 부여된 후 권한 서버가 사용자를 보내는 위치입니다. 인증 서버는 코드 또는 토큰을 리디렉션 URI로 전송하므로 앱 등록 프로세스의 일부로 올바른 위치를 등록하는 것이 중요합니다.

**응용 프로그램 프로비저닝**

[자습서: SCIM 끝점에 대한 프로비저닝 개발 및 계획](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) - 이 문서에서는 SCIM 끝점을 구축하고 AAD 프로비저닝 서비스와 통합하는 방법에 대해 설명합니다.


