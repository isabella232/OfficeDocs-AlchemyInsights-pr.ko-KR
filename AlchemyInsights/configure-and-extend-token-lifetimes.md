---
title: 토큰 수명 구성 및 연장
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 97e89feda45439dae59acca5817fdf359623d647997d08a5cbe4a6314fa6db3a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044922"
---
# <a name="configure-and-extend-token-lifetimes"></a>토큰 수명 구성 및 연장

Microsoft ID 플랫폼에서 발급한 액세스, SAML 또는 ID 토큰의 수명을 지정할 수 있습니다. 조직의 모든 앱, 다중 테넌트(여러 조직) 응용 프로그램 또는 조직의 특정 서비스 주체에 대해 토큰 수명을 설정할 수 있습니다. 자세한 내용은 [구성 가능한 토큰 수명](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)을 읽어 보세요.

예를 들어 [토큰 수명 구성 방법 예제](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes)를 참조하세요.

Azure AD B2C(Azure Active Directory B2C)에서 토큰의 수명 및 호환성을 구성하는 방법에 대한 자세한 내용은 [Azure Active Directory B2C에서 토큰 구성](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow)을 참조하세요.

[Azure Active Directory B2C에서 세션 동작 구성](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) 문서에서는 Azure AD B2C에서 사용되는 SSO(Single Sign-On) 방법을 설명하고 정책을 구성할 때 가장 적합한 SSO 방법을 선택하는 데 도움이 됩니다.

**토큰의 지속 기간 및 유효 기간**

토큰 수명은 1시간이고 세션 수명은 24시간입니다. 즉, 24시간 동안 요청이 없는 경우 새 토큰을 요청하기 전에 다시 로그인해야 합니다.

> [!NOTE]
> 2020년 5월 30일 이후에는 새 테넌트가 구성 가능한 토큰 수명 정책을 사용하여 세션 및 토큰을 구성할 수 없습니다. 그 후 몇 개월 이내에 더사용이 중단되며, 이는 곧 기존 세션에 대한 사용을 중단하고 토큰 정책을 새로 고치게 됩니다. 사용 중지 후에도 액세스 토큰 수명을 구성할 수 있습니다.






