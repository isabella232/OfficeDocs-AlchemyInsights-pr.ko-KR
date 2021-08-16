---
title: 자원 또는 서비스 보안 주체 관련 문제
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
- "9004336"
- "7741"
ms.openlocfilehash: 52b9b2e950d66c2f4105b76c4e2c70ed51320e4a57eb0008c353a9587fcc6510
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028082"
---
# <a name="issues-with-a-resource-or-service-principal"></a>자원 또는 서비스 보안 주체 관련 문제

1. 방금 시작한 경우 Azure Active Directory 응용 프로그램 및 서비스 주체 개체는 응용 프로그램 [등록,](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) 응용 프로그램 개체 및 서비스 Azure Active Directory, 응용 프로그램 개체의 사용 방법 및 서로의 관계에 대해 설명합니다. 응용 프로그램의 응용 프로그램 개체와 해당 서비스 사용자 개체 간의 관계를 설명하는 다중 테넌트 예제 시나리오도 제공합니다.
2. 에서 응용 프로그램 및 서비스 사용자 개체를 읽어 응용 프로그램과 서비스 사용자 간의 관계에 대해 [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
3. [방법:](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) 포털을 사용하여 리소스에 액세스할 수 있는 Azure AD 응용 프로그램 및 서비스 계정을 만드는 방법을 보여 Azure Active Directory(Azure AD) 응용 프로그램 및 서비스 계정을 역할 기반 액세스 제어에 사용할 수 있습니다.
4. 서비스 [주체 API를](https://docs.microsoft.com/graph/api/resources/serviceprincipal)사용하여 프로그래밍식으로 응용 프로그램 인스턴스를 관리하고 응용 프로그램이 테넌트 내에서 할 수 있는 작업을 제어할 수 있습니다.
5. [servicePrincipal 리소스 유형에는](https://docs.microsoft.com/graph/api/resources/serviceprincipal) servicePrincipal 리소스 유형에 대한 모든 속성과 메서드가 나열됩니다.
6. [Azure AD Graph Microsoft](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) Graph Azure AD Graph Microsoft Graph 차이점을 강조합니다. 이름이 다르거나 사용할 수 없는 리소스를 보여 주며, 또한 베타 버전의 Microsoft Graph v1.0 버전에서는 사용할 수 없는 리소스를 강조합니다.

**게스트 사용자 관련 문제**

- [빠른 시작: Azure Portal의](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) 디렉터리에 게스트 사용자를 추가하면 Azure Portal을 통해 Azure AD 디렉터리에 새 게스트 사용자를 추가하고, 초대를 보내고, 게스트 사용자의 초대 사용 프로세스가 어떻게 보이는지 확인할 수 있습니다.
- [자습서: B2C에서](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) 사용자 흐름을 Azure Active Directory Azure Portal을 사용하여 몇 가지 권장 사용자 흐름을 만드는 방법을 보여줍니다. 응용 프로그램에서 리소스 소유자 암호 자격 증명(ROPC) 흐름을 설정하는 방법에 대한 자세한 내용은 Azure AD B2C에서 리소스 소유자 암호 자격 증명 흐름 구성을 참조하세요.
