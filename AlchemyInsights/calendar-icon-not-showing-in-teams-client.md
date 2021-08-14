---
title: Teams 클라이언트에 일정 아이콘이 표시되지 않음
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 7881d6837cb7d99180d2cc1b28d327ce12e4b836d33e4fca099569d4f72510fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989597"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Teams 클라이언트에 일정 아이콘이 표시되지 않음

Teams의 일정 탭은 Exchange 웹 서비스를 통한 Exchange 사서함에 대한 액세스를 필요로합니다. Exchange 사서함은 온라인 이거나 온-프레미스 일 수 있습니다. 일정 탭이 표시되지 않는 온라인 사용자의 경우 [Exchange Online 사서함에 대한 라이선스가 부여되고 사서함이 사용하도록 설정](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes)되어 있는지 확인합니다.

사용자에게 Exchange Online의 유효한 사서함이 있지만 여전히 일정 탭이 표시되지 않는 경우 네트워크 문제일 수 있습니다. [Microsoft 원격 연결 분석기](https://testconnectivity.microsoft.com/)를 사용하여 영향받는 사용자에 대한 **Microsoft Exchange 웹 서비스 연결 테스트** 를 실행합니다.

마지막으로 [Teams 앱 – 앱 설정 정책](https://admin.teams.microsoft.com/policies/app-setup)을 통해 사용자에게 적용되는 정책에서 일정 앱이 제거되지 않았는지 확인합니다 **(전역(조직 전체의 기본값)일 가능성 높음**.

사용자가 온-프레미스에 있는 경우 하이브리드 구성이 정상인지 확인해야 합니다. [하이브리드 구성 마법사](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent)를 사용하여 문제를 해결하세요.

[Teams는 Exchange 2016 CU3 이상을 필요](https://docs.microsoft.com/microsoftteams/exchange-teams-interact)로 합니다.
