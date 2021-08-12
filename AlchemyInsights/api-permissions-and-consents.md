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
ms.openlocfilehash: c45bab67d414c8f0f2ca1c5275084d4ecce538c5256154292302080ba5bd8175
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932103"
---
# <a name="api-permissions-and-consent"></a>API 사용 권한 및 동의

응용 프로그램과 통합되는 Microsoft ID 플랫폼 권한 부여 모델을 따라 사용자와 관리자가 데이터에 액세스하는 방법을 제어할 수 있습니다. 권한 부여 모델의 구현이 끝점에서 Microsoft ID 플랫폼 업데이트되었습니다. 앱이 앱과 상호 작용하는 방식이 Microsoft ID 플랫폼. Microsoft ID 플랫폼 끝점의 사용 권한 및 동의에는 [범위,](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 사용 권한 및 동의를 포함하여 이 권한 부여 모델의 기본 개념이 설명되어 있습니다.

Azure [AZURE ACTIVE DIRECTORY](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) 동의 프레임워크를 사용하면 다중 테넌트 웹 및 네이티브 클라이언트 응용 프로그램을 쉽게 개발할 수 있습니다. 이러한 응용 프로그램을 사용하면 응용 프로그램이 등록된 Azure AD 테넌트의 사용자 계정으로 로그인할 수 있습니다. 또한 Microsoft Graph API(azure AD, Intune 및 Microsoft 365의 서비스에 액세스하기 위해) 및 기타 Microsoft 서비스' API와 같은 웹 API와 자체 웹 API에 액세스해야 할 수도 있습니다.

