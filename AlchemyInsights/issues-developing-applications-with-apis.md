---
title: API를 사용하는 응용 프로그램 개발 문제
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
- "9004343"
- "7755"
ms.openlocfilehash: 1de4e9aa5078507eecdbe53366e446e733029ecb1342f20ca701fa7f95a06fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013466"
---
# <a name="issues-developing-applications-with-apis"></a>API를 사용하는 응용 프로그램 개발 문제

Azure Active Directory Graph API 사용을 시작하거나 [Azure AD](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) Graph API 빠른 시작 가이드를 참조하거나 대화형 Azure AD Graph API [참조 설명서를 봐야 합니다.](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)

**ADAL(Azure Active Directory 인증 라이브러리) 및 Azure AD Graph API(AAD Graph) 지원 종료**

**2020년 6월 30일부터** 더 이상 ADAL 및 Azure AD 2013에 새로운 기능이 Graph. 기술 지원 및 보안 업데이트를 계속 제공하지만 기능 업데이트는 더 이상 제공하지 않습니다.

**2022년 6월 30일부터** ADAL 및 Azure AD Graph 지원이 종료될 예정으로, 더 이상 기술 지원 또는 보안 업데이트를 제공하지 않습니다.

기존 OS 버전에서 ADAL을 사용하는 앱은 이 시간 이후에도 계속 작동하지만 기술 지원이나 보안 업데이트를 받지 못합니다.

이 시간 이후 Azure AD Graph를 사용하는 앱은 더 이상 Azure AD Graph 끝점에서 응답을 받지 못할 수 있습니다.

**ADAL 마이그레이션**

최신 기능 및 보안 업데이트가 있는 [MSAL(Microsoft Authentication Library)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)로 업데이트하는 것이 좋습니다.

Microsoft 앱을 사용하는 경우 Microsoft가 지원 종료 기한까지 응용 프로그램을 MSAL로 마이그레이션하는 중이라는 것을 알고 MSAL의 지속적인 보안 및 기능 개선을 통해 혜택을 받을 수 있습니다.

1. [ADAL FAQ를 읽어보세요](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [플랫폼별로 앱을 마이그레이션하는 방법을 알아보세요](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. ADAL을 사용하는 앱을 이해하는 데 도움이 필요한 경우 모든 앱의 소스 코드를 검토하고 해당하는 경우 ISV 또는 앱 공급자에게 도움을 드리는 것이 좋습니다. 또한 Microsoft 지원을 통해 테넌트에 있는 Microsoft가 아닌 모든 ADAL 앱 목록을 제공할 수 있습니다.

**AAD 그래프 마이그레이션**

Azure AD 앱을 사용하는 응용 Graph 지침에 따라 Azure AD Graph [앱을 Microsoft](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)Graph.

1. [마이그레이션 점검표를 통해 시작 지점 제공](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist) 
1. Azure 앱 등록 포털에 AAD 그래프를 사용하는 응용 프로그램이 표시됩니다. 모든 앱의 소스 코드를 검토하고 해당되는 경우 ISV 또는 앱 공급자에게 문의하는 것이 좋습니다. Microsoft 지원은 테넌트의 모든 AAD Graph 제공할 수도 있습니다.
1. 앱에서 Microsoft Graph 데이터에 액세스하려면 사용자 또는 관리자가 동의 프로세스를 통해 올바른 사용 권한을 부여해야 합니다. Microsoft [Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) 권한 참조에는 각 주요 Microsoft Graph API와 연결된 사용 권한이 나열됩니다. 또한 사용 권한을 사용하는 방법에 대한 지침도 제공합니다.
