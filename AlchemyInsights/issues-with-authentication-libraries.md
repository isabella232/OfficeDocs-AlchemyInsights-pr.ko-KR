---
title: 인증 라이브러리 관련 문제
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
- "9004333"
- "7731"
ms.openlocfilehash: 39336fa8840a28befcad449d0afa59c1df5c6bef5988cb197916a03aa2aa66c9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028010"
---
# <a name="issues-with-authentication-libraries"></a>인증 라이브러리 관련 문제

1. [Microsoft ID 플랫폼 라이브러리에는](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) Microsoft에서 지원되는 호환되는 클라이언트 및 미들웨어 라이브러리가 나열됩니다.
2. MSAL(Microsoft 인증 라이브러리)은 [](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) 다양한 응용 프로그램 시나리오에서 사용할 수 있는 여러 인증 흐름을 지원합니다.
3. 토큰을 인증하고 획득하기 위해 코드에서 새 공용 또는 기밀 클라이언트 응용 프로그램을 초기화합니다. MSAL(Microsoft 인증 라이브러리)에서 클라이언트 앱을 초기화할 때 여러 구성 옵션을 설정할 수 있습니다. 자세한 내용은 응용 프로그램 구성 [옵션 을 참조하세요.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)

**ADAL(Azure Active Directory 인증 라이브러리) 및 Azure AD Graph API(AAD Graph) 지원 종료**

**2020년 6월 30일부터** 더 이상 ADAL 및 Azure AD 2013에 새로운 기능이 Graph. 기술 지원 및 보안 업데이트를 계속 제공하지만 기능 업데이트는 더 이상 제공하지 않습니다.

**2022년 6월 30일부터** ADAL 및 Azure AD Graph 지원이 종료될 예정으로, 더 이상 기술 지원 또는 보안 업데이트를 제공하지 않습니다.

기존 OS 버전에서 ADAL을 사용하는 앱은 이 시간 이후에도 계속 작동하지만 *기술 지원이나 보안 업데이트* 를 받지 못합니다.

이 시간 이후 Azure AD Graph를 사용하는 앱은 더 이상 Azure AD Graph 끝점에서 응답을 받지 못할 수 있습니다.

**ADAL 마이그레이션**

최신 기능 및 보안 업데이트가 있는 [MSAL(Microsoft Authentication Library)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)로 업데이트하는 것이 좋습니다.

Microsoft 앱을 사용하는 경우 Microsoft가 지원 종료 기한까지 MSAL로 응용 프로그램을 마이그레이션하는 중이라는 것을 알고 MSAL의 지속적인 보안 및 기능 개선을 통해 혜택을 받을 수 있습니다.

자세한 내용은 다음 항목을 참조하세요.

1. [ADAL FAQ 읽기](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [플랫폼별로 앱을 마이그레이션하는 방법 알아보기](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. ADAL을 사용하는 앱을 이해하는 데 도움이 필요한 경우 모든 앱의 소스 코드를 검토하고 해당하는 경우 ISV 또는 앱 공급자에게 도움을 드리는 것이 좋습니다. 또한 Microsoft 지원을 통해 테넌트에 있는 Microsoft가 아닌 모든 ADAL 앱 목록을 제공할 수 있습니다.

**AAD 그래프 마이그레이션**

Azure AD 앱을 사용하는 응용 Graph 지침에 따라 Azure AD Graph [앱을 Microsoft](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)Graph.

1. [마이그레이션 검사 목록은 시작 지점을 제공합니다.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Azure 앱 등록 포털에 AAD 그래프를 사용하는 응용 프로그램이 표시됩니다. 모든 앱의 소스 코드를 검토하고 해당되는 경우 ISV 또는 앱 공급자에게 문의하는 것이 좋습니다. Microsoft 지원은 테넌트의 모든 AAD Graph 제공할 수도 있습니다.
3. 앱에서 Microsoft Graph 데이터에 액세스하려면 사용자 또는 관리자가 동의 프로세스를 통해 올바른 사용 권한을 부여해야 합니다. Microsoft [Graph](https://docs.microsoft.com/graph/permissions-reference) 권한 참조에는 각 주요 Microsoft Graph API와 연결된 사용 권한이 나열됩니다. 또한 사용 권한을 사용하는 방법에 대한 지침도 제공합니다.
