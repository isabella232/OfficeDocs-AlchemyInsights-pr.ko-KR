---
title: 구독 액세스
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
- "9003799"
- "6805"
ms.openlocfilehash: b138c05e87e70c18bb6528819a34f8a9501446d57dcf4dbac0734f70fbc3466b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999246"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>브라우저 문제로 인해 Azure에 로그인할 수 없습니다(브라우저 중단, 계속 회전, 로드되지 않는 등).

정전의 영향을 을 수 있습니다. 지속적인 정전이 있는 경우 Azure Health [Status를 참조하세요.](https://status.azure.com/status/history/)

모든 활성 Azure 세션에서 로그아웃하세요. 웹 브라우저의 비공개 또는 시코그니치 모드를 시작하세요.

위의 브라우저가 작동하지 않는 경우 브라우저 새로 고침, 다른 브라우저 사용, 캐시 쿠키 삭제를 시도할 수도 있습니다.

자세한 내용은 [다음을(를) 통해 로그인 문제 해결을 위한 정보를 제공합니다.](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**구독에 액세스할 수 없습니다.**

Azure [Portal에서](https://portal.azure.com/)오른쪽 위에 있는 계정에서 올바른 Azure 디렉터리가 선택되어 있는지 확인합니다.

Azure [계정 센터에서](https://account.windowsazure.com/Subscriptions)사용된 계정이 계정 관리자인지 확인 합니다.

자세한 내용은 [다음을(를) 선택합니다. 구독을 찾을 수 없음 문제 해결](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**청구 내역에 액세스할 수 없습니다.**

계정 관리자는 청구 정보에 액세스하는 사용자가 Azure Active Directory에 게스트 사용자인 새 사용자 추가 또는 삭제를 [추가하는지 확인해야 합니다.](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)

그런 다음 사용자에게 전역 관리자 역할 할당 을 [부여해야 합니다.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)

이 게시 사용자에게 RBAC 정책을 사용하여 청구 액세스 권한을 부여할 수 있습니다. 대금 [청구에 대한 액세스](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)권한 부여.

**추천 문서**

-   [Azure 구독을 관리하기 위해 로그인할 수 없습니다.](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)