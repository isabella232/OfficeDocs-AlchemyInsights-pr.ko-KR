---
title: 사용자 동의 문제 해결
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: db784c133fec554604ad09f5b27941879d97ff238f926ff6338d0f3b7c3c4105
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007904"
---
# <a name="troubleshoot-user-consent"></a>사용자 동의 문제 해결

1. Azure Portal 또는 PowerShell을 통해 최종 사용자가 응용 프로그램에 동의하는 방법을 구성할 수 있습니다. 자세한 [내용은 사용자 동의](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) 설정을 참조하세요.
1. 관리자는 Microsoft Graph [API를](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) 사용하여 단일 사용자를 대신하여 위임된 사용 권한에 대한 동의를 부여할 수도 있습니다. 자세한 내용은 사용자 대신 액세스 를 [참조하세요.](https://docs.microsoft.com/graph/auth-v2-user)
1. [사용자 동의](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)오류: 이 문서에서는 응용 프로그램에 동의하는 프로세스 중에 발생할 수 있는 오류에 대해 논의합니다. 오류 메시지가 없는 예기치 않은 동의 프롬프트 문제를 해결하는 경우 Azure AD에 대한 [인증 시나리오를 참조하세요.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)