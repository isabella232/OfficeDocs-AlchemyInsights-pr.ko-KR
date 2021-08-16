---
title: 인증 문제
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7748"
- "9004339"
ms.openlocfilehash: c7e6d96940f8d7052ee4b49b22c0d1d7d5bd5f9277f4a7eff709def1da2e13af
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019514"
---
# <a name="authentication-issues"></a>인증 문제

**Azure AD(Azure Active Directory) STS(보안 토큰 서비스)에서 반환되는 AADS 오류 코드에 대한 정보를 찾고 계신가요?** AADSTS 오류 설명, 수정 및 제안된 해결 방법을 찾으려면 [Azure AD 인증 및 인증 오류 코드](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes)를 참조하세요.

인증 오류는 401 또는 403 오류를 생성하는 여러 가지 문제로 인해 발생할 수 있습니다. 예를 들어 다음과 같은 문제가 모두 권한 부여 오류로 이어질 수 있습니다.

- 잘못된 [액세스 토큰 획득 흐름](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- 잘못된 [권한 범위 구성](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- [동의](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent) 부족

일반적인 권한 부여 오류를 해결하려면 수신되는 오류와 가장 일치하는 아래 단계를 시도해 보세요. 수신 중인 오류에 대해 둘 이상의 단계가 적용될 수 있습니다.

**401 Unauthorized error: 토큰이 유효한가요?**

앱이 요청의 일부로 Microsoft Graph에 유효한 액세스 토큰을 제공하고 있는지 확인합니다. 이 오류는 종종 액세스 토큰이 HTTP 인증 요청 헤더에 없거나 토큰이 잘못되었거나 만료되었음을 의미합니다. 액세스 토큰 획득에 MSAL(Microsoft Authentication Library)을 사용하는 것이 좋습니다. 또한 개인 Microsoft 계정에 부여된 위임 액세스 토큰을 사용하여 회사 또는 학교 계정(조직 계정)만 지원하는 API에 액세스하려고 하면 이 오류가 발생할 수 있습니다.

**403 Forbidden error: 올바른 권한 세트를 선택했나요?**

앱에서 호출하는 Microsoft Graph API를 기반으로 올바른 권한 집합을 요청했는지 확인합니다. 권장 최소 권한 사용 권한은 모든 Microsoft Graph API 참조 방법 항목에서 제공됩니다. 또한 이러한 권한은 사용자 또는 관리자가 응용 프로그램에 부여해야 합니다. 권한 부여는 일반적으로 동의 페이지 또는 Azure Portal 응용 프로그램 등록 블레이드의 사용을 통해 이루어집니다. 응용 프로그램에 대한 **설정** 블레이드에서 **필수 권한** 을 클릭하고 **권한 허용** 을 클릭합니다. 자세한 내용은 다음을 참조하세요.

- [Microsoft Graph 사용 권한](https://docs.microsoft.com/graph/permissions-reference) 
- [Azure AD 사용 권한 및 동의 이해](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**403 Forbidden error: 앱에서 선택한 권한과 일치하는 토큰을 획득했나요?**

요청하거나 부여된 권한 유형이 앱에서 획득한 액세스 토큰 유형과 일치하는지 확인하세요. 앱 사용 권한을 요청 및 부여하지만 클라이언트 자격 증명 흐름 토큰 대신 위임된 대화형 코드 흐름 토큰을 사용하거나, 위임된 사용 권한을 요청 및 부여하지만 위임된 코드 흐름 토큰 대신 클라이언트 자격 증명 흐름 토큰을 사용할 수 있습니다.

토큰 수집과 관련된 자세한 내용은 다음을 참조하세요.

- [사용자 및 위임된 사용 권한을 대신하여 액세스 권한 부여](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v2.0 - OAuth 2.0 인증 코드 흐름](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [사용자(데몬 서비스) 및 응용 프로그램 사용 권한 없이 액세스 가능](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v2.0 - OAuth 2.0 클라이언트 자격 증명 흐름](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**403 Forbidden error: 암호 재설정**

현재 사용자 암호를 재설정할 수 있는 응용 프로그램 권한 데몬 서비스 대 서비스 권한이 없습니다. 이러한 API는 로그인한 관리자가 있는 대화형 위임 코드 흐름만 사용할 수 있습니다. 자세한 내용은 [Microsoft Graph 사용 권한](https://docs.microsoft.com/graph/permissions-reference)을 참조하세요.

**403 Forbidden: 사용자에게 액세스 권한이 있으며 라이선스가 부여되나요?**

위임된 코드 흐름의 경우 Microsoft Graph는 앱에 부여된 권한과 로그인한 사용자가 가진 권한을 기준으로 요청이 허용되었는지 여부를 평가합니다. 일반적으로 이 오류는 사용자가 요청을 수행할 수 있는 권한이 없는 경우 **또는** 액세스 중인 데이터에 대한 라이센스가 없음을 나타냅니다. 필요한 권한 또는 라이선스를 가진 사용자만 성공적으로 요청을 수행할 수 있습니다.

**403 Forbidden: 올바른 리소스 API를 선택했나요?**

Microsoft Graph와 같은 API 서비스는 수신된 액세스 토큰의 *aud* 클레임(청중)이 스스로 기대하는 값과 일치하는지 확인하고, 그렇지 않으면 403 Forbidden error가 발생합니다. 이 오류가 발생하는 일반적인 오류는 Azure AD Graph API, Outlook API 또는 SharePoint/OneDrive API에 대해 획득한 토큰을 사용하여 Microsoft Graph를 호출하거나 그 반대입니다. 앱에서 토큰을 획득하는 리소스(또는 범위)가 앱이 호출하는 API와 일치하는지 확인합니다.

**400 Bad Request or 403 Forbidden: 사용자가 조직의 CA(조건부 액세스) 정책을 준수하나요?**

조직의 CA(조건부 액세스) 정책에 따라 앱을 통해 Microsoft Graph 리소스에 액세스하는 사용자에게 앱이 처음 획득한 액세스 토큰에 없는 추가 정보가 필요할 수 있습니다. 이 경우 액세스 토큰을 획득할 때 **400 *interaction_required*** 오류를 받거나 Microsoft Graph를 호출할 때 **403 *insufficient_claims*** 를 받습니다. 두 경우 모두 오류 응답에는 사용자에게 다단계 인증 또는 장치 등록과 같은 추가 정보를 요청하기 위해 인증된 끝점에 표시할 수 있는 추가 정보가 포함됩니다.

조건부 액세스와 관련된 자세한 내용은 다음을 참조하세요.

- [MSAL을 사용하여 조건부 액세스 문제 처리](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Azure Active Directory 조건부 액세스에 대한 개발자 가이드](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

***ADAL(Azure Active Directory 인증 라이브러리) 및 AZure AD 그래프 API(AAD Graph) 지원 종료***

- 2020년 6월 30일부터 ADAL(Azure Active Directory 인증 라이브러리) 및 AAD 그래프 API(Azure AD Graph API)에 새로운 기능을 더 이상 추가하지 않습니다. 기술 지원 및 보안 업데이트를 계속 제공하지만 기능 업데이트는 더 이상 제공하지 않습니다.
- 2022년 6월 30일부터 ADAL 및 AAD Graph에 대한 지원을 종료하고 더 이상 기술 지원이나 보안 업데이트를 제공하지 않습니다.
    - 기존 OS 버전에서 ADAL을 사용하는 앱은 이 시간 이후에도 계속 작동하지만 기술 지원이나 보안 업데이트를 받지 못합니다.
    - 이 시간 이후 AAD 그래프를 사용하는 앱은 더 이상 AAD 그래프 엔드포인트에서 응답을 받지 못할 수 있습니다.

**ADAL 마이그레이션**

최신 기능 및 보안 업데이트가 있는 [MSAL(Microsoft Authentication Library)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)로 업데이트하는 것이 좋습니다. 이 권장 사항은 Microsoft가 지원 종료 시한까지 응용 프로그램을 MSAL로 마이그레이션하는 경우에 해당합니다. Microsoft 앱을 MSAL로 마이그레이션하는 목적은 앱이 MSAL의 지속적인 보안 및 기능 향상의 혜택을 받기 위한 것입니다.

- [ADAL FAQ 읽기](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [플랫폼별로 앱을 마이그레이션하는 방법 알아보기](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- ADAL을 사용하는 앱을 이해하는 데 도움이 필요한 경우 모든 앱의 소스 코드를 검토하고 해당하는 경우 ISV(독립 소프트웨어 벤더) 또는 앱 공급자에게 문의하는 것이 좋습니다. 또한 Microsoft 지원을 통해 테넌트에 있는 Microsoft가 아닌 모든 ADAL 앱 목록을 제공할 수 있습니다.

**AAD 그래프 마이그레이션**

AAD 그래프를 사용하는 응용 프로그램의 경우 다음 지침에 따라 [Azure AD Graph 응용 프로그램을 Microsoft Graph로 마이그레이션](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true)하세요.

- [마이그레이션 점검표를 통해 시작 지점 제공](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist) 
- Azure 앱 등록 포털에 AAD 그래프를 사용하는 응용 프로그램이 표시됩니다. 모든 앱의 소스 코드를 검토하고 해당되는 경우 ISV 또는 앱 공급자에게 문의하는 것이 좋습니다. 또한 Microsoft 지원은 테넌트의 모든 AAD 그래프 사용에 대한 정보를 제공할 수 있습니다.

 










