---
title: API 사용 권한 및 동의
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
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49951922"
---
# <a name="api-permissions-and-consent"></a>API 사용 권한 및 동의

Microsoft ID 플랫폼과 통합되는 응용 프로그램은 사용자와 관리자가 데이터 액세스 방법을 제어할 수 있는 권한 부여 모델을 따르게 됩니다. 권한 부여 모델의 구현이 Microsoft ID 플랫폼 끝점에서 업데이트되었습니다. 앱이 Microsoft ID 플랫폼과 상호 작용하는 방식이 변경됩니다. [Microsoft ID 플랫폼](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 끝점의 사용 권한 및 동의에는 범위, 사용 권한 및 동의를 포함하여 이 권한 부여 모델의 기본 개념이 설명됩니다.

[Azure AD(Azure Active Directory)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) 동의 프레임워크를 사용하면 다중 테넌트 웹 및 기본 클라이언트 응용 프로그램을 쉽게 개발할 수 있습니다. 이러한 응용 프로그램은 응용 프로그램이 등록된 계정과는 다른 Azure AD 테넌트의 사용자 계정으로 로그인할 수 있도록 허용합니다. Microsoft Graph API(Microsoft 365의 Azure AD, Intune 및 서비스에 액세스하기 위해) 및 기타 Microsoft 서비스의 API와 같은 웹 API와 자체 웹 API에 액세스해야 할 수도 있습니다.

