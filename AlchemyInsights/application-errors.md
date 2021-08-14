---
title: 응용 프로그램 오류
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "7841"
ms.openlocfilehash: ce4c89da79112726ed4fb25527edc8d082bd37f239595b9eab7279abeeecfd7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931455"
---
# <a name="application-errors"></a>응용 프로그램 오류

STS(Azure AD) 보안 토큰 서비스(Azure Active Directory)에서 반환되는 **AADSTS** 오류 코드에 대한 정보를 찾고 있나요? AADSTS Azure AD 인증 설명, 수정 및 제안된 해결 방법을 찾아보는 오류 코드 및 권한 부여 오류 코드를 읽어 읽습니다. [](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes)

인증 오류는 401 또는 403 오류를 생성하는 여러 가지 문제로 인해 발생할 수 있습니다. 예를 들어 다음이 모두 권한 부여 오류가 발생할 수 있습니다.

- 잘못된 [액세스 토큰 획득 흐름](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- 잘못된 [권한 범위 구성](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- [동의](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent) 부족

일반적인 권한 부여 오류를 해결하려는 경우 아래 제공된 단계를 수행하여 수신하는 오류와 가장 일치하는지 확인하십시오. 두 개 이상 적용될 수 있습니다.

**401 Unauthorized error: 토큰이 유효한가요?**

응용 프로그램이 요청의 일부로 Microsoft Graph 액세스 토큰을 제공해야 합니다. 이 오류는 종종 액세스 토큰이 HTTP 인증 요청 헤더에 없거나 토큰이 잘못되었거나 만료되었음을 의미합니다. 액세스 토큰 획득을 위해 [MSAL(Microsoft 인증 라이브러리)을](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) 사용하는 것이 좋습니다. 또한 개인 Microsoft 계정에 부여된 위임된 액세스 토큰을 사용하여 직장 또는 학교 계정(조직 계정)만 지원하는 API에 액세스하려는 경우 이 오류가 발생할 수 있습니다.

**403 Forbidden error: 올바른 권한 세트를 선택했나요?**

앱에서 호출하는 Microsoft Graph API에 따라 올바른 사용 권한 집합을 요청해야 합니다. 권장되는 최소 권한 사용 권한은 모든 Microsoft Graph API 참조 메서드 항목에서 제공됩니다. 또한 이러한 권한은 사용자 또는 관리자가 응용 프로그램에 부여해야 합니다. 사용 권한 부여는 일반적으로 동의 페이지 또는 Azure Portal 응용 프로그램 등록 블레이드를 사용하여 사용 권한을 부여하여 발생합니다. 응용 프로그램에 대한 **설정** 블레이드에서 **필수 권한** 을 클릭하고 **권한 허용** 을 클릭합니다.

- [Microsoft Graph 사용 권한](https://docs.microsoft.com/graph/permissions-reference) 
- [Azure AD 사용 권한 및 동의 이해](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**403 Forbidden error: 앱에서 선택한 권한과 일치하는 토큰을 획득했나요?**

요청되거나 부여된 권한 유형이 앱에서 획득하는 액세스 토큰 유형과 일치하는지 확인 응용 프로그램 권한을 요청 및 부여하지만 클라이언트 자격 증명 흐름 토큰 대신 위임된 대화형 코드 흐름 토큰을 사용하거나, 위임된 코드 흐름 토큰 대신 클라이언트 자격 증명 흐름 토큰을 사용하여 위임된 사용 권한을 요청 및 부여할 수 있습니다.

- [사용자 및 위임된 사용 권한을 대신하여 액세스 권한 부여](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v2.0 - OAuth 2.0 인증 코드 흐름](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [사용자(데몬 서비스) 및 응용 프로그램 사용 권한 없이 액세스 가능](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v2.0 - OAuth 2.0 클라이언트 자격 증명 흐름](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**403 Forbidden error: 암호 재설정**

현재 사용자 암호를 재설정할 수 있는 응용 프로그램 권한 데몬 서비스 대 서비스 권한이 없습니다. 이러한 API는 로그인한 관리자가 있는 대화형 위임 코드 흐름만 사용할 수 있습니다.

- [Microsoft Graph 사용 권한](https://docs.microsoft.com/graph/permissions-reference)

**403 Forbidden: 사용자에게 액세스 권한이 있으며 라이선스가 부여되나요?**

위임된 코드 흐름의 경우 Microsoft Graph 앱에 부여된 사용 권한 및 로그인한 사용자가 부여한 사용 권한에 따라 요청이 허용되는지 평가합니다. 일반적으로 이 오류는 사용자가 요청을 수행할 수 있는 권한이 없는 경우 또는 액세스 중인 데이터에 대한 라이센스가 없음을 나타냅니다. 필요한 권한 또는 라이선스를 가진 사용자만 성공적으로 요청을 수행할 수 있습니다.

**403 Forbidden: 올바른 리소스 API를 선택했나요?**

Microsoft Graph 같은 API 서비스는 수신된 액세스 토큰의 수신된 클레임(대상) 값이 자체적으로 예상한 값과 일치하는지 확인하고 그렇지 않은 경우 403 금지 오류가 발생합니다. 이 오류가 발생하는 일반적인 오류는 Azure AD Graph API, Outlook API 또는 SharePoint/OneDrive API에 대해 획득한 토큰을 사용하여 Microsoft Graph를 호출하거나 그 반대입니다. 앱에서 토큰을 획득하는 리소스(또는 범위)가 앱이 호출하는 API와 일치하는지 확인합니다.

**400 Bad Request or 403 Forbidden: 사용자가 조직의 CA(조건부 액세스) 정책을 준수하나요?**

조직의 CA 정책에 따라 앱을 통해 Microsoft Graph 리소스에 액세스하는 사용자에게 앱의 원래 획득한 액세스 토큰에 없는 추가 정보가 필요하게 될 수 있습니다. 이 경우 액세스 토큰을 획득할 때 400 *interaction_required* 오류를 받거나 Microsoft Graph를 호출할 때 403 *insufficient_claims* 를 받습니다. 두 경우 모두 오류 응답에는 사용자에게 추가 정보(예: 다단계 인증 또는 장치 등록)를 요청하도록 승인 끝점에 제공될 수 있는 추가 정보가 포함되어 있습니다.

- [MSAL을 사용하여 조건부 액세스 문제 처리 ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Azure Active Directory 조건부 액세스에 대한 개발자 가이드](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
