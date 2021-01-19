---
title: 로그 아웃 문제
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7793"
- "9004355"
ms.openlocfilehash: 794e5c43340ba4b5c653eda4c11b4480cd3fa710
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886842"
---
# <a name="sign-out-issues"></a>로그 아웃 문제

로그 아웃과 관련된 문제는 다음 단계를 수행합니다.

1. 사용자나 사용자가 응용 프로그램에서 로그아웃되거나 종료되는 경우 [조건별 액세스를 사용하여 인증 세션 관리 구성"](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime)또는 [Microsoft ID 플랫폼에서 토큰 수명 구성](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)의 지침을 따르세요.
2. 다른 대부분의 로그아웃 오류 또는 문제는 Azure AD(Azure Active Directory)를 특정 응용 프로그램과 통합하는 문제를 해결하여 해결할 수 있습니다. 다음을 포함한 [Azure Active Directory와 애플리케이션을 통합하기 위한 자습서 모음](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)으로 이동하여 특정 통합에 대한 지침을 확인할 수 있습니다.
    - SaaS 응용 프로그램 자습서
    - Single Sign-On 자습서
    - 사용자 프로비저닝 자습서