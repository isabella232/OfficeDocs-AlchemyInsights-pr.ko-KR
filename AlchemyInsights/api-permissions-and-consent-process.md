---
title: API 사용 권한 및 동의 프로세스
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "9200"
ms.openlocfilehash: 078f5798533dfbbf97858f305729f103663644fee3590cdcc877233041adae81
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932067"
---
# <a name="api-permissions-and-consent-process"></a>API 사용 권한 및 동의 프로세스

앱에서 Microsoft Graph 데이터에 액세스하려면 사용자 또는 관리자가 동의 프로세스를 통해 올바른 사용 권한을 부여해야 합니다. [Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 권한 참조에는 각 주요 Microsoft Graph API와 연결된 사용 권한이 나열됩니다. 또한 사용 권한을 사용하는 방법에 대한 지침도 제공합니다.

**서비스 보안 주체 설정 또는 업데이트**

- [Create serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - 이 문서에서는 새 servicePrincipal 개체를 만드는 방법을 보여줍니다.
- [포털에서 Azure AD](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) 앱 & 서비스 사용자 만들기 - 이 문서에서는 역할 기반 액세스 제어에 사용할 수 있는 새 Azure Active Directory(Azure AD) 응용 프로그램 및 서비스 계정을 만드는 방법을 보여줍니다.
- [Azure AD의](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) & 앱 - 이 문서에서는 응용 프로그램 등록, 응용 프로그램 개체 및 서비스 보안 주체에 대해 Azure Active Directory 방법, 사용 방법 및 서로 관련되는 방식에 대해 설명합니다.

**앱 등록 추가 또는 업데이트 및 관리자 동의 제공**

- [앱 등록 만들기](https://docs.microsoft.com/graph/api/application-post-applications) - 이 문서에서는 새 응용 프로그램 개체를 만드는 방법을 보여줍니다.
- [앱 등록 업데이트 - API 권한](https://docs.microsoft.com/graph/api/application-update) - 이 문서에서는 응용 프로그램 개체의 속성을 업데이트하는 방법을 보여줍니다.
- [관리자 동의 제공](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - 일반적으로 관리자 동의 및 동의를 위해서는 관리자가 명시적으로 동의를 부여해야 합니다.
- [RBAC(베타)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - 단일 역할 할당에서 여러 보안 주체와 여러 범위를 지원하는 Microsoft 365 RBAC 공급자에 대한 통합 역할 정의 및 역할 할당에 대한 역할 관리 컨테이너입니다. 이는 *rbacApplication* 리소스 유형과 다릅니다. Microsoft Intune RBAC 공급자의 예입니다. Intune의 역할 할당에는 보안 주체 배열과 범위 그룹 배열이 있습니다. **베타 버전이며, 이는 아직 개발 중이며 프로덕션에서 사용하기에 권장되지 않음을 의미합니다.**
