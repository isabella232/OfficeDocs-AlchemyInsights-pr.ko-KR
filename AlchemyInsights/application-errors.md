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
ms.openlocfilehash: 2ef90b54ce222a06740e05891fabe87b6565cb14
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49976915"
---
# <a name="application-errors"></a>응용 프로그램 오류

Azure AD(Azure Active Directory) STS(보안 토큰 서비스)에서 반환되는 **AADSTS** 오류 코드에 대한 정보를 찾고 있나요? [Azure AD 인증](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 및 권한 부여 오류 코드를 읽고 AADSTS 오류 설명, 수정 내용 및 제안된 해결 방법을 찾을 수 있습니다.

권한 부여 오류는 여러 가지 문제로 인해 발생할 수 있습니다. 이로 인해 대부분 401 또는 403 오류가 발생합니다. 예를 들어 다음이 모두 권한 부여 오류가 발생할 수 있습니다.

- 잘못된 [액세스 토큰 취득 흐름](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- 잘못 구성된 [사용 권한 범위](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- 동의 [부족](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

일반적인 권한 부여 오류를 해결하려는 경우 아래 제공된 단계를 수행하여 수신하는 오류와 가장 일치하는 단계를 시도합니다. 두 개 이상 적용될 수 있습니다.

**401 권한이 없는 오류: 토큰이 유효한지 여부**

응용 프로그램에서 요청의 일부로 유효한 액세스 토큰을 Microsoft Graph에 표시해야 합니다. 이 오류는 종종 HTTP 인증 요청 헤더에 액세스 토큰이 누락되었거나 토큰이 유효하지거나 만료된 것일 수 있습니다. 액세스 토큰 취득에는 [MSAL(Microsoft 인증](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) 라이브러리)을 사용하는 것이 좋습니다. 또한 개인 Microsoft 계정에 부여된 위임된 액세스 토큰을 사용하여 직장 또는 학교 계정(조직 계정)만 지원하는 API에 액세스하려는 경우 이 오류가 발생할 수 있습니다.

**403 금지된 오류: 올바른 사용 권한 집합을 선택합니까?**

앱에서 호출하는 Microsoft Graph API를 기반으로 올바른 사용 권한 집합을 요청한지 확인합니다. 권장되는 최소 권한 사용 권한은 모든 Microsoft Graph API 참조 메서드 항목에서 제공됩니다. 또한 사용자 또는 관리자가 해당 사용 권한을 응용 프로그램에 부여해야 합니다. 일반적으로 사용 권한 부여는 동의 페이지 또는 Azure Portal 응용 프로그램 등록 블레이드를 사용하여 사용 권한을 부여하여 발생합니다. 응용 프로그램의 **설정** 블레이드에서 필요한 사용 권한을 클릭한 다음 사용 권한 **부여를 클릭합니다.**

- [Microsoft Graph 사용 권한](https://docs.microsoft.com/graph/permissions-reference) 
- [Azure AD 사용 권한 및 동의 이해](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**403 금지된 오류: 앱이 선택한 사용 권한과 일치하기 위해 토큰을 획득했습니까?**

요청되거나 부여된 권한 유형이 앱에서 획득하는 액세스 토큰 유형과 일치하는지 확인 응용 프로그램 권한을 요청 및 부여하지만 클라이언트 자격 증명 흐름 토큰 대신 위임된 대화형 코드 흐름 토큰을 사용하거나, 위임된 사용 권한을 요청 및 부여하지만 위임된 코드 흐름 토큰 대신 클라이언트 자격 증명 흐름 토큰을 사용할 수 있습니다.

- [사용자 및 위임된 사용 권한을 대신하여 액세스 권한 부여](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v2.0 - OAuth 2.0 권한 부여 코드 흐름](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [사용자(데몬 서비스) 및 응용 프로그램 권한 없이 액세스](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v2.0 - OAuth 2.0 클라이언트 자격 증명 흐름](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**403 금지된 오류: 암호 다시 설정**

현재 사용자 암호를 다시 설정할 수 있는 응용 프로그램 권한 데몬 서비스-서비스 권한은 없습니다. 이러한 API는 로그인한 관리자와의 대화형 위임 코드 흐름을 사용하여만 지원됩니다.

- [Microsoft Graph 사용 권한](https://docs.microsoft.com/graph/permissions-reference)

**403 금지: 사용자에게 액세스 권한이 있으며 라이선스가 있습니까?**

위임된 코드 흐름의 경우 Microsoft Graph는 앱에 부여된 사용 권한 및 로그인한 사용자가 부여한 사용 권한에 따라 요청이 허용되는지 평가합니다. 일반적으로 이 오류는 사용자에게 요청을 수행할 수 있는 권한이 충분하지 않은 경우 또는 액세스되는 데이터에 대한 사용이 허가되지 않았다는 것을 나타냅니다. 필요한 사용 권한 또는 라이선스가 있는 사용자만 요청을 성공적으로 만들 수 있습니다.

**403 금지: 올바른 리소스 API를 선택했습니까?**

Microsoft Graph와 같은 API 서비스는 수신된 액세스 토큰의 수신된 클레임(대상) 값이 자체적으로 예상한 값과 일치하는지 확인하며, 그렇지 않은 경우 403 금지 오류가 발생합니다. 이 오류가 발생하는 일반적인 실수는 Azure AD Graph API, Outlook API 또는 SharePoint/OneDrive API에 대해 획득한 토큰을 사용하여 Microsoft Graph(또는 그 반대의 경우)를 호출하려고 하는 것입니다. 앱에서 토큰을 확보하는 리소스(또는 범위)가 앱이 호출하는 API와 일치하는지 확인

**400 잘못된 요청 또는 403 금지: 사용자가 조직의 CA(조건부 액세스) 정책을 준수하나요?**

조직의 CA 정책에 따라 앱을 통해 Microsoft Graph 리소스에 액세스하는 사용자는 앱이 원래 구입한 액세스 토큰에 없는 추가 정보에 대해 의문을 던지게 될 수 있습니다. 이 경우 앱은 액세스 토큰을 취득하는 *동안* interaction_required 오류가 발생하거나 Microsoft Graph를 호출할  때 insufficient_claims 오류가 있는 400을 수신합니다. 두 경우 모두 오류 응답에는 사용자에게 추가 정보(예: 다단계 인증 또는 장치 등록)를 요청하도록 승인 끝점에 제공될 수 있는 추가 정보가 포함되어 있습니다.

- [MSAL을 사용하여 조건부 액세스 문제 처리 ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Azure Active Directory 조건부 액세스에 대한 개발자 지침](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
