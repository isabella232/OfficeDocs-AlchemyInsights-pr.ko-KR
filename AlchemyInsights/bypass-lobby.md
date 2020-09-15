---
title: 바이패스 로비
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
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684956"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>팀에서의 로비 설정 및 참여 수준 제어

전화 접속, 외부 및 익명 사용자를 포함 하 여 모든 사용자가 **로비를 우회**하도록 허용 하려면 PowerShell을 사용 하 여이 작업을 수행 합니다. 다음은 조직에 대 한 전역 모임 정책을 수정 하는 예입니다.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

이 cmdlet은 현재 비즈니스용 Skype PowerShell 모듈을 사용 해야 합니다. 이 cmdlet을 사용 하도록 설정 하려면 [PowerShell을 통해 정책 관리](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)를 참조 하세요.

정책을 설정한 후에는 사용자에 게 적용 해야 합니다. 또는 전역 정책을 수정한 경우 사용자에 게 자동으로 적용 됩니다. 정책이 변경 되는 경우 정책이 적용 되려면 최소 **24** 시간까지 기다려야 합니다. 

이를 변경 하기 전에 아래의 설명서를 검토 하 여 해당 작업을 정확히 이해 해야 합니다.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>팀 모임 로비 정책 컨트롤 이해

이러한 설정은 모임에 참가 하기 전에 로비에서 대기 하는 모임 참가자 및 모임에서 허용 되는 참여 수준을 제어 합니다. PowerShell을 사용 하 여 팀 관리 센터에서 아직 구현 되지 않은 모임 정책 설정 ("출시 예정")을 업데이트할 수 있습니다. 모든 사용자가 로비를 무시할 수 있도록 하는 예제 PowerShell cmdlet은 아래를 참조 하십시오.

- 사용자가 인증 된 사용자가 참석할 수 있을 때까지 사용자가 모임에 직접 참가 하거나 로비에서 대기할지 여부를 제어 하는 이끌이 별 정책 [으로 자동으로 인정](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) 합니다.

- [익명 사용자가 모임을 시작할 수 있도록 허용](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) 은 B2B 및 페더레이션 사용자를 비롯 한 익명 사용자가 사용자의 모임에 참석할 수 있는지 여부를 제어 하는 이끌이 별 정책입니다.

- 전화 [접속 사용자의 로비 사용 허용](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**출시 예정**)은 전화로 전화를 거는 사용자가 모임에 직접 참가할 지 또는 **자동 허용 사용자** 설정에 관계 없이 로비에서 대기할지 여부를 제어 하는 이끌이 별 정책입니다.

- [이끌이가 로비 설정 재정의 허용](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**곧 예정**)은 모임 이끌이가 관리자가 **자동으로 사용자** **를 허용 하 고 전화 접속 사용자가** 새 모임을 예약할 때 로비를 우회 하도록 할 수 있는지 여부를 제어 하는 이끌이 별 정책입니다.

**참고:** Microsoft 팀 회의 정책에 대 한 전체 개요를 보려면 [팀에서 모임 정책 관리](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) 를 참조 하세요.
