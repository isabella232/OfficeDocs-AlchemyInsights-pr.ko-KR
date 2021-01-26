---
title: 응용 프로그램 개발 문제
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
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950802"
---
# <a name="issues-developing-applications"></a>응용 프로그램 개발 문제

Azure AD(Active Directory) 앱을 만들 때 가장 일반적인 문제를 해결하려면 다음 문서를 참조하세요.

- [Chrome 브라우저만 사용하여 응용 프로그램에 로그인하는 데 문제가 있는 경우](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [응용 프로그램의 토큰 수명 기본값을 변경하는 방법을 모르는 경우](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [응용 프로그램 동의 작동 방식을 헷갈리는 경우](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [응용 프로그램에 사용 권한을 부여하는 방법을 모르는 경우](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [위임된 권한과 응용 프로그램 권한의 차이를 이해할 수 없는 경우](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***ADAL(Azure Active Directory 인증 라이브러리) 및 AZure AD 그래프 API(AAD Graph) 지원 종료** _

- 2020년 6월 30일부터 ADAL(Azure Active Directory 인증 라이브러리) 및 AAD 그래프 API(Azure AD Graph API)에 새로운 기능을 더 이상 추가하지 않습니다. 기술 지원 및 보안 업데이트를 계속 제공하지만 기능 업데이트는 더 이상 제공하지 않습니다.

- 2022년 6월 30일부터 ADAL 및 AAD Graph에 대한 지원을 종료하고 더 이상 기술 지원이나 보안 업데이트를 제공하지 않습니다. 이 상태로 인해 다음과 같은 결과가 나타납니다.

    - 기존 OS 버전에서 ADAL을 사용하는 앱은 이 시간 이후에도 계속 작동하지만 기술 지원이나 보안 업데이트를 받지 못합니다.

    - 이 시간 이후 AAD 그래프를 사용하는 앱은 더 이상 AAD 그래프 엔드포인트에서 응답을 받지 못할 수 있습니다.

_ *ADAL 마이그레이션**

Microsoft 앱을 사용하는 경우 최신 기능 및 보안 업데이트가 있는 MSAL(Microsoft Authentication Library)로 업데이트하는 것이 좋습니다. 이 권장 사항은 Microsoft가 지원 종료 시한까지 응용 프로그램을 MSAL로 마이그레이션하는 프로세스를 시작한 경우에 해당합니다. 

Microsoft의 응용 프로그램을 MSAL로 마이그레이션하면 MSAL의 지속적인 보안 및 기능 향상의 이점을 얻을 수 있습니다.

1. [ADAL FAQ 읽기](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [플랫폼별로 앱을 마이그레이션하는 방법 알아보기](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. ADAL을 사용하는 앱을 이해하는 데 도움이 필요한 경우 모든 앱의 소스 코드를 검토하고 해당하는 경우 ISV(독립 소프트웨어 벤더) 또는 앱 공급자에게 문의하는 것이 좋습니다. 또한 Microsoft 지원을 통해 테넌트에 있는 Microsoft가 아닌 모든 ADAL 앱 목록을 제공할 수 있습니다.

**AAD 그래프 마이그레이션**

AAD 그래프를 사용하는 응용 프로그램의 경우 다음 지침에 따라 AAD 그래프 응용 프로그램을 Microsoft Graph로 마이그레이션하세요.

1. [마이그레이션 점검표를 통해 시작 지점 제공](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist) 
2. Azure 앱 등록 포털에 AAD 그래프를 사용하는 응용 프로그램이 표시됩니다. 모든 앱의 소스 코드를 검토하고 해당하는 경우 ISV(독립 소프트웨어 벤더) 또는 앱 공급자에게 문의하는 것이 좋습니다. 또한 Microsoft 지원은 테넌트의 AAD 그래프 사용에 대한 정보를 제공할 수 있습니다.







