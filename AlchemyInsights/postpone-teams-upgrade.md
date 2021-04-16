---
title: Teams 업그레이드 연기
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
ms.openlocfilehash: abbf696b1554743bda188704272bfd85fe6f94e2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51801237"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a>Microsoft 주도 Teams 업그레이드를 연기하는 방법

**중요:** 지원 진단을 사용하여 이 문제를 해결할 수 있지만 새 관리 센터를 사용하지 않는 것 같습니다. 새 관리 센터를 사용하려면 오른쪽 위에 새 관리  센터가 표시됩니다. 새 관리 센터를 사용하여 도움이 **필요하세요?** 위젯을 클릭하고 "Teams 업그레이드 연기"를 입력한 다음 프롬프트에 따라 진단을 실행합니다.

비즈니스용 Skype에서 Microsoft Teams로의 Microsoft 주도 자동 업그레이드에 대한 통신을 받았고 자동화된 업그레이드를 나중에 연기하려면 전역 관리자가 [Teams](https://admin.teams.microsoft.com/dashboard) 관리 포털에 로그인하고 Microsoft Teams 업그레이드에서 상태  새로 고침 단추를 선택한 후 연기 단추를 선택합니다.  테넌트가 Microsoft Teams로 자동 업그레이드하는 새 날짜를 확인하려면 Teams 관리 포털 페이지를 새로 고치십시오.

**참고:** 연기 **단추는** 자동화된 업그레이드와 관련하여 메시지 센터 알림을 받은 경우만 사용할 수 있습니다. 

전역 관리자는 [Get-CsTeamsUpgradeStatus를](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) 실행하여 현재 업그레이드 상태에 대해 자세히 확인할 수도 있습니다.
