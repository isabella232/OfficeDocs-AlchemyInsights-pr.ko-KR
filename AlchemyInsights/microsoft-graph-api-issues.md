---
title: Microsoft Graph API 문제
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
- "9004345"
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/29/2021
ms.locfileid: "50716200"
---
# <a name="microsoft-graph-api-issues"></a>Microsoft Graph API 문제

이 항목은 여전히 Azure AD Graph API를 사용하는 개발자에게도 적용될 수 있습니다. 그러나 모든  디렉터리, ID 및 액세스 관리 시나리오에 Microsoft Graph를 사용하는 것이 좋습니다.

**인증 또는 권한 부여 문제**

- 앱에서 Microsoft  Graph를 호출하는 토큰을 얻을 수 없는 경우 이 항목에 대한 자세한 도움말과 지원을 확인하려면 액세스 토큰(인증) Microsoft Graph 범주를 사용하는 데 문제가 있는 경우를 선택합니다. 
- 앱에서 Microsoft Graph를 호출할 때 **401 또는 403** 권한 부여 오류가 발생하는 경우 액세스 거부 오류 보기(권한 **부여)** Microsoft Graph API 범주를 선택해 이 항목에 대한 보다 구체적인 도움말 및 지원을 얻습니다.

**Microsoft Graph를 사용하지만 어디서 시작해야 할지 잘 모르겠다**

- [Microsoft Graph 개요](https://docs.microsoft.com/graph/overview)
- [Microsoft Graph의 ID 및 액세스 관리 개요](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Microsoft Graph 앱 구축 시작](https://docs.microsoft.com/graph/)
- **Microsoft Graph 탐색기** - 테넌트 또는 데모 테넌트에서 Microsoft Graph API 테스트

**Microsoft Graph를 사용하지만 필요한 v1.0 디렉터리 API를 지원하나요?**

디렉터리, ID 및 액세스 관리에 권장되는 API는 Microsoft Graph입니다. 그러나 Azure AD Graph와 Microsoft Graph 간에는 여전히 몇 가지 간격이 있습니다. 다음 문서를 검토하여 선택에 도움이 될 최신 차이점을 중점적으로 다듬습니다.

- [Azure AD Graph와 Microsoft Graph 간의 리소스 유형 차이](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Azure AD Graph와 Microsoft Graph의 속성 차이](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Azure AD와 Microsoft Graph의 메서드 차이](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**호출하는 API가 작동하지 않습니다. 더 많은 테스트를 어디서 할 수 있나요?**

**Microsoft Graph 탐색기** - 테넌트 또는 데모 테넌트에서  Microsoft Graph API를 테스트하고 Microsoft Graph 탐색기에서 샘플 쿼리도 확인 합니다.

**내 앱이 너무 느리며 또한 스로틀링됩니다. 개선할 수 있는 기능**

시나리오에 따라 다양한 옵션을 사용하여 응용 프로그램의 실행을 높일 수 있으며, 경우에 따라 서비스에서 스로틀링하기 까다로우기 까다로우며(너무 많은 전화를 걸 때) 다양한 옵션을 사용할 수 있습니다.

- [Microsoft Graph 모범 사례](https://docs.microsoft.com/graph/best-practices-concept)
- [일괄 처리 요청](https://docs.microsoft.com/graph/json-batching)
- [델타 쿼리를 통해 변경 내용 추적](https://docs.microsoft.com/graph/delta-query-overview)
- [webhook을 통해 변경 내용에 대한 알림을 받을 수 있습니다.](https://docs.microsoft.com/graph/webhooks)
- [스로틀 지침](https://docs.microsoft.com/graph/throttling)

**오류 및 알려진 문제에 대한 자세한 내용은 어디에서 찾을 수 있나요?**

- [Microsoft Graph 오류 응답 정보](https://docs.microsoft.com/graph/errors)
- [Microsoft Graph의 알려진 문제](https://docs.microsoft.com/graph/known-issues)

**서비스 가용성 및 연결 상태를 어디에서 확인할 수 있나요?**

Microsoft Graph를 통해 액세스할 수 있는 서비스 가용성 및 연결성은 Microsoft Graph의 전반적인 가용성 및 성능에 영향을 줄 수 있습니다.

- Azure Active Directory 서비스 상태의 경우 Azure 상태 페이지에 나열된 **보안 + ID** 서비스의 상태를 [확인합니다.](https://azure.microsoft.com/status/)
- Microsoft Graph에 참여하는 Office 서비스의 경우 Office 서비스 상태 대시보드에 나열된 서비스의 [상태를 확인 합니다.](https://portal.office.com/adminportal/home#/servicehealth)

Microsoft Graph 권한 부여 오류는 여러 가지 문제로 인해 발생할 수 있습니다. 이로 인해 대부분 401 또는 403 오류가 발생합니다. 예를 들어 다음이 모두 권한 부여 오류가 발생할 수 있습니다.

- 잘못된 [액세스 토큰 획득 흐름](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- 잘못된 [권한 범위 구성](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- [동의](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent) 부족

**_ADAL(Azure Active Directory 인증 라이브러리) 및 AZure AD 그래프 API(AAD Graph) 지원 종료_* _

_*2020년 6월 30일**부터는 더 이상 ADAL 및 Azure AD Graph에 새 기능을 추가하지 않습니다. 기술 지원 및 보안 업데이트를 계속 제공하지만 기능 업데이트는 더 이상 제공하지 않습니다.

**2022년 6월 30일부터** ADAL 및 Azure AD Graph에 대한 지원이 종료될 예정으로, 더 이상 기술 지원 또는 보안 업데이트를 제공하지 않습니다.

기존 OS 버전에서 ADAL을 사용하는 앱은 이 시간 이후에도 계속 작동하지만 기술 지원 또는 보안 업데이트는 받을 *수 없습니다.*

이 시간이 지난 후 Azure AD Graph를 사용하는 앱은 더 이상 Azure AD Graph 끝점에서 응답을 받지 않을 수 있습니다.

**ADAL 마이그레이션**

최신 기능 및 보안 업데이트가 있는 [MSAL(Microsoft Authentication Library)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)로 업데이트하는 것이 좋습니다.

Microsoft 앱을 사용하는 경우 Microsoft가 지원 종료 기한까지 응용 프로그램을 MSAL로 마이그레이션하는 중이라는 것을 알고 MSAL의 지속적인 보안 및 기능 개선을 통해 혜택을 받을 수 있습니다.

1. [ADAL FAQ 읽기](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [플랫폼별로 앱을 마이그레이션하는 방법 알아보기](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. ADAL을 사용하는 앱을 이해하는 데 도움이 필요한 경우 모든 앱의 소스 코드를 검토하고 해당하는 경우 ISV 또는 앱 공급자에게 도움을 드리는 것이 좋습니다. 또한 Microsoft 지원을 통해 테넌트에 있는 Microsoft가 아닌 모든 ADAL 앱 목록을 제공할 수 있습니다.

**AAD 그래프 마이그레이션**

Azure AD Graph를 사용하는 응용 프로그램의 경우 지침에 따라 Azure AD Graph 앱을 [Microsoft Graph로 마이그레이션합니다.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [마이그레이션 점검표를 통해 시작 지점 제공](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Azure 앱 등록 포털에 AAD 그래프를 사용하는 응용 프로그램이 표시됩니다. 모든 앱의 소스 코드를 검토하고 해당되는 경우 ISV 또는 앱 공급자에게 문의하는 것이 좋습니다. Microsoft 지원은 테넌트의 모든 AAD Graph 사용 목록을 제공할 수도 있습니다.
3. 앱에서 Microsoft Graph의 데이터에 액세스하려면 사용자 또는 관리자가 동의 프로세스를 통해 올바른 사용 권한을 부여해야 합니다. [Microsoft Graph 사용 권한 참조에는](https://docs.microsoft.com/graph/permissions-reference) 각 주요 Microsoft Graph API 집합과 연결된 사용 권한이 나열됩니다. 또한 사용 권한을 사용하는 방법에 대한 지침도 제공합니다.
