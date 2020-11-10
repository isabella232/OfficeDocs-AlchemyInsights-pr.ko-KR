---
title: 팀 대화에서 Giphys 사용
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
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947514"
---
# <a name="using-giphys-in-teams-conversations"></a>팀 대화에서 Giphys 사용

Giphys에서 팀 채팅에 대 한 액세스는 기본적으로 사용 하도록 설정 됩니다. 관리자는 [메시징 정책을 설정](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) 하 고 **대화에서 Giphys 사용** 이 **켜져** 있는지 확인 하 여 사용자가 Giphys를 사용할 수 있는지 여부를 제어할 수 있습니다.

Gif가 팀 대화에서 예상 대로 작동 하지 않는 경우에는 다음을 확인 합니다.

[메시징 정책이](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) Giphys를 허용 해야 합니다. PowerShell cmdlet을 사용 하 여 확인 하려면

- [PowerShell을 사용 하 여 팀을 관리할](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)수 있는지 확인 합니다.
- PowerShell 명령 [CsTeamsMessagingPolicy-Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) 을 실행 하 고 **AllowGiphy** 이 **TRUE** 로 설정 되어 있는지 확인 합니다.
- **AllowGiphy** 가 **FALSE** 로 설정 된 경우 다음 PowerShell 명령 CsTeamsMessagingPolicy- [AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps)를 실행 합니다.

Giphy URL에 대 한 액세스를 허용 하려면 [연결 된 선택적 환경을](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) 사용 하도록 설정 해야 합니다.

> [!NOTE]
> 테 넌 트에 대해 여러 팀 메시징 정책이 구성 된 경우 PowerShell 명령 [get-csonlineuser-identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) |를 사용 하 여 영향을 받는 사용자에 게 할당 된 정책의 id를 확인할 수 있습니다. <user@domain.com> TeamsMessagingPolicy를 선택 합니다.
