---
title: 업그레이드 Teams 연기
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
- "2737"
- "4000006"
ms.openlocfilehash: 893a01ae74f8aec9bb0079430188e3cd6881b3009818830ea5572cfa41cdf71f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923983"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a>Microsoft 주도 업그레이드를 연기하는 Teams 방법

**중요:** 지원 진단을 사용하여 이 문제를 해결할 수 있지만 새 관리 센터를 사용하지 않는 것 같습니다. 새 관리 센터를 사용하려면 오른쪽 위에 새 관리  센터가 표시됩니다. 새 관리 센터를 사용하여 도움이 **필요하세요?** 위젯을 클릭하고 "업그레이드 연기Teams 프롬프트에 따라 진단을 실행합니다.

비즈니스용 Skype에서 Microsoft Teams로의 Microsoft 주도 자동 업그레이드에 대한 통신을 받았고 자동화된 업그레이드를 나중에 연기하려면 전역 관리자가 [Teams](https://admin.teams.microsoft.com/dashboard) 관리 포털에 로그인하고 Microsoft Teams 업그레이드에서 상태 새로  고침 단추를 선택한 후  연기 단추를 선택합니다. 테넌트의 자동 업그레이드 날짜를 확인하려면 Microsoft Teams 관리 포털 페이지를 Teams 새로 고쳐야 합니다.

**참고:** 연기 **단추는** 자동화된 업그레이드와 관련하여 메시지 센터 알림을 받은 경우만 사용할 수 있습니다. 

전역 관리자는 [Get-CsTeamsUpgradeStatus를](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) 실행하여 현재 업그레이드 상태에 대해 자세히 확인할 수도 있습니다.
