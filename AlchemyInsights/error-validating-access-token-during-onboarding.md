---
title: Desktop Analytics를 접속하는 동안 액세스 토큰 오류 유효성 검사 오류가 발생했습니다.
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813694"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Desktop Analytics 온보더링 중에 "액세스 토큰 유효성 검사 오류가 발생했습니다." 오류

이 오류는 일반적으로 인증 토큰이 만료될 때 관찰됩니다. 일반적으로 페이지를 새로 고치면 토큰이 새로 고쳐지게 됩니다. 그러나 Desktop Analytics를 사용하는 계정에 적용되는 조건부 액세스 정책이 있는 경우 이 문제가 지속될 수 있습니다. Azure Portal의 Azure AD 로그인 로그를 검토하여 Desktop Analytics 등록에 사용되는 계정에 대한 로그인 오류가 없는지 볼 수 있습니다.

조건부 액세스에 대한 자세한 내용은 [Plan your Conditional Access deployment을 참조하십시오.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)