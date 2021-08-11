---
title: 앱 등록 클라이언트 비밀 또는 인증서 문제
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
- "9004352"
- "9685"
ms.openlocfilehash: 588273f43f7c2d57b377b234885cf4283d466919b562536f78a64356422f9f9f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951499"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>앱 등록 클라이언트 비밀 또는 인증서 문제

응용 프로그램 클라이언트 비밀 만료 여부

앱 등록 포털의 표준 등록 프로세스를 통해 또는 응용 프로그램 동의를 사용하여 테넌트에서 서비스 계정을 만든 경우 등록된 응용 프로그램을 만든 방식에 관계없이 현재 클라이언트 보안이 만료 전에 새 클라이언트 비밀을 만들어 관련 응용 프로그램 코드에서 업데이트해야 합니다. 최대 유효 기간은 2년입니다. 미리 알림으로 비밀 값은 포털에서 앱 등록 페이지를 종료한 후 더 이상 표시되지 않는 것으로 기록해야 합니다. 자세한 내용은 빠른 [시작:](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) Microsoft ID 플랫폼 앱 등록 및 앱에 대한 모범 [사례를 Microsoft ID 플랫폼.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)

자세한 내용은 [Create an Azure AD app & service principal in the portal - Microsoft ID 플랫폼.](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)
