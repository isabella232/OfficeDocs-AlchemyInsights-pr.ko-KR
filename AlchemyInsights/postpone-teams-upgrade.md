---
title: 팀 업그레이드 연기
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
- "2737"
- "4000006"
ms.openlocfilehash: ae0611df247790200d0192e018ff5f0128f23cb4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741777"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a>Microsoft 기반 팀 업그레이드를 연기 하는 방법

**중요**: 지원 진단을 사용 하 여이 문제를 해결할 수는 있지만 새 관리 센터를 사용 하 고 있지 않은 것 같습니다. 새 관리 센터를 사용 하려면 **새 관리 센터** 를 표시 하는 오른쪽 위 단추를 오른쪽 위로 밀어 둡니다. 새 관리 센터를 사용 하 여 **도움이 필요 하신가요?** widget을 클릭 하 고 "팀 업그레이드 연기"를 입력 한 다음 화면의 지시에 따라 진단 프로그램을 실행 합니다.

비즈니스용 Skype에서 microsoft 팀으로 Microsoft 연동 자동 업그레이드에 대 한 통신을 받은 경우, 자동 업그레이드를 나중 날짜로 연기 하려면 전역 관리자가 [팀 관리 포털](https://admin.teams.microsoft.com/dashboard) 에 로그인 하 고 Microsoft 팀 업그레이드에서 **상태 새로 고침** 단추를 선택한 후 **연기** 단추를 선택 합니다. Microsoft 팀에 대 한 테 넌 트의 자동 업그레이드에 대 한 새 날짜를 보려면 팀 관리 포털 페이지를 새로 고칩니다.

**참고:** **연기** 단추는 자동화 된 업그레이드에 대 한 메시지 센터 알림을 받은 경우에만 사용할 수 있습니다. 

전역 관리자는 [CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) 를 실행 하 여 현재 업그레이드 상태에 대해 자세히 알아볼 수도 있습니다.
