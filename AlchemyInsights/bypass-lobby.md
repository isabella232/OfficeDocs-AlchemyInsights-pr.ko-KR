---
title: 대기실 우회
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
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820040"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>대기실 설정 및 Teams 참여 수준 제어

전화 접속, 외부 및 익명 사용자를 비롯한 모든 사용자가 대기실을 우회하도록 허용할 경우 PowerShell을 사용하여 이 작업을 수행할 수 있습니다.  다음은 조직의 전역 모임 정책을 수정하는 예입니다.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

이 cmdlet은 현재 비즈니스용 Skype PowerShell 모듈을 사용해야 합니다. 이 cmdlet을 사용하기 위한 설정은 [PowerShell을](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)통해 정책 관리를 확인 합니다.

정책을 설정한 후 사용자에게 적용해야 합니다. 또는 글로벌 정책을 수정한 경우 자동으로 사용자에게 적용됩니다. 정책이 변경될 경우 정책이 적용될 때까지 **최소 4시간에서 최대 24시간을** 기다려야 합니다. 

이러한 변경을 통해 허용하는 내용을 정확하게 이해하기 전에 아래 설명서를 검토해야 합니다.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Teams 모임 대기실 정책 컨트롤 이해

이러한 설정은 모임에 참가하기 전에 대기실에서 대기하는 모임 참가자와 모임에 참가할 수 있는 참가 수준을 제어합니다. PowerShell을 사용하여 Teams 관리 센터에서 아직 구현되지 않은 모임 정책 설정("출시 예정"으로 표시)을 업데이트할 수 있습니다. 모든 사용자가 대기실을 우회할 수 있도록 하는 예제 PowerShell cmdlet은 아래를 참조하세요.

- [자동으로 사용자](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) 입력은 사용자가 직접 모임에 참가할지 또는 인증된 사용자가 참가할 때까지 대기실에서 대기할지 여부를 제어하는 이끌이 정책입니다.

- [익명 사용자가](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) 모임을 시작할 수 있도록 허용은 B2B 및 페더니트 사용자를 비롯한 익명 사용자가 조직의 인증된 사용자가 참석하지 않고 사용자의 모임에 참가할 수 있는지 여부를 제어하는 이끌이 정책입니다.

- [전화 접속](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) 사용자가 대기실을 우회하도록 허용(곧 출시 예정)은 전화 접속한 사용자가 자동으로 사용자 허용 설정에 관계없이 전화로 모임에 직접 참가할지 또는 대기실에서 대기하는지 여부를 제어하는 이끌이 **정책입니다.** 

- [이끌이가](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) 대기실 설정을 무시하도록 허용(출시 예정)은 모임 이끌이가 자동으로 사용자 허용 및 전화 접속 사용자가  새 모임을  예약할 때 대기실을 무시하도록 허용에서 설정한 대기실 설정을 무시할 수 있는지 여부를 제어하는 이끌이 정책입니다.

**참고:** Microsoft [Teams 모임 정책에](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) 대한 전체 개요는 Teams에서 모임 정책 관리를 참조하세요.
