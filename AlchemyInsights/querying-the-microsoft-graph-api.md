---
title: Microsoft Graph API 쿼리
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
- "7846"
ms.openlocfilehash: eda5d8d1d76d0d87312b1441aeae89d8e250abe0e8b613d4a43fcc2345a6f021
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923245"
---
# <a name="querying-the-microsoft-graph-api"></a>Microsoft Graph API 쿼리

이 항목은 여전히 Azure AD api를 사용하는 개발자에게 Graph 있습니다. 그러나 모든  디렉터리, ID 및 액세스 관리 시나리오에 Graph Microsoft 365를 사용하는 것이 좋습니다.

**인증 또는 권한 부여 문제**

- 앱에서 Microsoft  Graph 호출하는 토큰을 얻을 수 없는 경우 이 항목에 대한 자세한 도움말과 지원을 Graph **Microsoft** Graph 범주를 다운로드하는 데 문제가 있습니다.
- 앱에서 Microsoft Graph 호출할 때 **401 또는 403** 권한 부여 오류가 발생하는 경우 액세스 거부 오류(권한 **부여)** Microsoft Graph API 범주를 선택해 이 항목에 대한 보다 구체적인 도움말과 지원을 얻습니다.

**Microsoft Graph 사용하지만 어디서 시작해야 할지 잘 모르겠음**

Microsoft Graph 자세한 내용은 다음을 참조합니다.

- [Microsoft Graph 개요](https://docs.microsoft.com/graph/overview)
- [Microsoft 365의 ID 및 액세스 관리 Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Microsoft Graph 앱 구축 시작](https://docs.microsoft.com/graph/)
- **Microsoft Graph 탐색기** - 테넌트 또는 데모 Graph Microsoft Graph API 테스트

**Microsoft Graph 사용하지만 필요한 v1.0 디렉터리 API를 지원하나요?**

Microsoft Graph, ID 및 액세스 관리에 권장되는 API입니다. 그러나 Azure AD 2013과 Microsoft Graph 간에는 여전히 몇 가지 Graph. 다음 문서를 검토하여 선택에 도움이 될 최신 차이점을 중점적으로 다듬습니다.

- [Azure AD와 Microsoft Graph 리소스 유형 Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Azure AD와 Microsoft Graph 속성 Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Azure AD와 Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**사용자 개체를 *쿼리할* 때 많은 속성이 누락되었습니다.**

`GET https://graph.microsoft.com/v1.0/users`Microsoft는 반환할 기본 Graph 자동으로 선택하기 때문에 11개  속성만 반환합니다. 다른 사용자 *속성이* 필요한 경우 $select 응용 프로그램에 필요한 속성을 선택하십시오. **먼저 Microsoft** Graph 사용해 보아야 합니다.

**일부 사용자 속성 값은 설정되어 있는 것을 *알고도 null입니다.***

응용 프로그램에 *User.ReadBasic.All* 권한이 부여된 것이 가장 큰 설명입니다. 이렇게 하면 응용 프로그램에서 제한된 사용자 속성 집합을 읽을 수 있습니다. 이 경우 다른 모든 속성은 이전에 설정한 경우에도 null로 반환됩니다. 대신 응용 프로그램 *User.Read.All* 사용 권한을 부여해 보아야 합니다.

자세한 내용은 Microsoft Graph [권한을 참조하세요.](https://docs.microsoft.com/graph/permissions-reference#user-permissions)

**OData 쿼리 매개 변수를 사용하여 요청의 데이터를 필터링하는 데 문제가 있습니다.**

Microsoft Graph 다양한 OData 쿼리 매개 변수를 지원하기는 하지만 이러한 매개 변수 중 상당수는 Microsoft 365의 디렉터리 *서비스(directoryObject에서* 상속하는 리소스)에서 완전히 지원되지 Graph. Azure AD 2013에 제공된 동일한 제한 Graph Microsoft 365에서 가장 Graph.

1. **지원되지**$count, $search 및 $filter *null* 값에 대해 지원되지 *않습니다.*
2. **지원되지**$filter 속성에 대한 정보(필터링할 수 있는 속성에 대한 리소스 항목 참조)
3. **지원되지 않는** 경우: 동시에 포징, 필터링 및 정렬
4. **지원되지 않는** 경우: 관계에 대한 필터링. 예 - 영국에 있는 엔지니어링 그룹의 모든 구성원을 찾을 수 있습니다.
5. **부분 지원**: $orderby(displayName 및 userPrincipalName만 해당) 및 *그룹에 대해* 지원 
6. **부분** 지원 : $filter ( *eq,* *시작* 또는 , 및 제한 *)* 지원, $expand(단일 개체의 관계를 확장하면 모든 관계가 반환되지만 개체의 관계 컬렉션 확장은 제한)

자세한 내용은 쿼리 매개 [변수를 사용하여 응답 사용자 지정을 참조하세요.](https://docs.microsoft.com/graph/query-parameters)

**호출하는 API가 작동하지 않습니다. 더 많은 테스트를 할 수 있는 곳은 어디인가요?**

**Microsoft Graph 탐색기** - 테넌트 또는 데모 테넌트에서 Microsoft Graph API를  테스트하고 Microsoft Graph 탐색기에서 샘플 쿼리를 확인 합니다.

**데이터를 쿼리할 때 불완전한 데이터 집합이 다시 있는 것 같습니다.**

사용자와 같은 컬렉션을 쿼리하는 경우 Microsoft Graph 페이지 제한을 사용하여 결과가 항상 기본 페이지 크기로 반환됩니다.  앱은 항상 서비스에서 반환된 컬렉션을 통해 페이지로 이동해야 합니다.

자세한 내용은 다음 항목을 참조하세요.

- [Microsoft Graph 모범 사례](https://docs.microsoft.com/graph/best-practices-concept)
- [앱에서 Microsoft Graph 데이터 포징](https://docs.microsoft.com/graph/paging)

**내 앱이 너무 느리며 또한 스로틀링됩니다. 개선할 수 있는 기능**

시나리오에 따라 다양한 옵션을 사용하여 응용 프로그램의 실행을 높일 수 있으며, 경우에 따라 서비스로의 스로틀링을 덜 덜 수도 있습니다(너무 많은 호출을 하는 경우).

자세한 내용은 다음을 참조하세요:

- [Microsoft Graph 모범 사례](https://docs.microsoft.com/graph/best-practices-concept)
- [일괄 처리 요청](https://docs.microsoft.com/graph/json-batching)
- [델타 쿼리를 통해 변경 내용 추적](https://docs.microsoft.com/graph/delta-query-overview)
- [webhook을 통해 변경 내용에 대한 알림을 받을 수 있습니다.](https://docs.microsoft.com/graph/webhooks)
- [스로틀 지침](https://docs.microsoft.com/graph/throttling)

**오류 및 알려진 문제에 대한 자세한 내용은 어디에서 찾을 수 있나요?**

- [Microsoft Graph 오류 응답 정보](https://docs.microsoft.com/graph/errors)
- [Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**서비스 가용성 및 연결 상태를 어디에서 확인할 수 있나요?**

Microsoft 365를 통해 액세스할 수 있는 서비스 가용성 및 연결성은 Microsoft Graph 전반적인 가용성 및 성능에 영향을 줄 수 Graph.

- 서비스 Azure Active Directory Azure 상태 페이지에 나열된 보안 **+ ID** 서비스의 [상태를 확인하십시오.](https://azure.microsoft.com/status/)
- Microsoft Office 서비스에 Graph 서비스 상태 대시보드 에 나열된 서비스 Office [확인 합니다.](https://portal.office.com/adminportal/home#/servicehealth)
