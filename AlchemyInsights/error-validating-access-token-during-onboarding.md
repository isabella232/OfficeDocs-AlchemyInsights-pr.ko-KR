---
title: 데스크톱 분석을 통해 온-탑재 중에 액세스 토큰 오류 유효성을 검사 하는 동안 오류가 발생 했습니다.
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783557"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Desktop Analytics 온 보 딩 중 "액세스 토큰 유효성을 검사 하는 동안 오류가 발생 했습니다." 오류

이 오류는 일반적으로 인증 토큰이 만료 되는 경우에 관찰 됩니다. 일반적으로 페이지를 새로 고치면 토큰이 새로 고쳐집니다. 그러나 온보드 데스크톱 분석에 사용 되는 계정에 조건부 액세스 정책이 적용 된 경우에는이 문제가 지속 될 수 있습니다. Azure Portal에서 Azure AD 로그인 로그를 검토 하 여 데스크톱 분석 온 보 딩에 사용 중인 계정에 대 한 로그인 오류가 있는지 확인할 수 있습니다.

조건부 액세스에 대 한 자세한 내용은 [조건부 액세스 배포 계획](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)을 참조 하십시오.