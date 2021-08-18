---
title: 대화에서 giphy Teams 사용
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
- "9003825"
- "6850"
ms.openlocfilehash: 296c2f80d35f1c93ab3c60e0be65fd96c953ca81
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323526"
---
# <a name="using-giphys-in-teams-conversations"></a>대화에서 giphy Teams 사용

Teams 채팅의 Giphy 액세스는 기본적으로 사용하도록 설정되어 있습니다. 관리자는 메시징 정책을 설정하고 대화에서 Giphys [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) 사용이 설정 으로 설정 하여 **사용자에게 Giphy를** 사용할 수 있는지 제어할 수 **있습니다.**

GIF가 대화에서 예상대로 작동하지 Teams 다음을 확인 합니다.

메시징 [정책에서](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) Giphy를 허용해야 합니다. PowerShell cmdlet을 사용하여 확인:

- [PowerShell을](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)사용하여 관리 Teams 수 있는지 확인
- PowerShell 명령 [Get-CsTeamsMessagingPolicy -Identity Global을](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) 실행하고 **AllowGiphy가** TRUE로 설정되어 있는지 **확인해야 합니다.**
- **AllowGiphy가** **FALSE로** 설정된 경우 다음 PowerShell 명령 [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps)$True.

[선택적 연결된 환경을](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) 사용하도록 설정해야 Giphy URL에 액세스할 수 있습니다.

**참고:** 테넌트에 대해 Teams 메시징 정책을 여러 개 구성한 경우 PowerShell 명령 [Get-CsOnlineUser -Identity를](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) 사용하여 영향을 받을 사용자에게 할당된 정책의 ID를 확인할 <user@domain.com> 수 | TeamsMessagingPolicy를 선택합니다.
