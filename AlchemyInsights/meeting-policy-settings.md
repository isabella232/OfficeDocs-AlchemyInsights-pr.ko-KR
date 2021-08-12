---
title: 모임 정책 설정
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
- "9000734"
- "2657"
ms.openlocfilehash: 06395bcc1a631adeaa8abb5ad63b971639f226c19e48203078ba1097d43a50f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925171"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>모임 정책 관리 Microsoft Teams

**참고: 정책 변경 내용이 사용자에게 적용될 경우 최대 24시간이 걸릴 수 있습니다.** 새로 만든 정책을 즉시 변경하지 못하게 될 수 있습니다. 4시간을 기다렸다가 새로 만든 정책을 다시 수정하려고 합니다.

모임 정책은 조직에서 사용자들이 예약한 모임에 대하여 해당 참가자에게 제공되는 기능을 제어하는 데 사용됩니다. 모임 정책의 일부 기능은 아직 Teams 관리 센터에서 구현되지 않을 수 있습니다(설명서에서 "곧 제공될 예정"으로 레이블이 지정되어 있습니다). 이 경우 또는 Microsoft Teams 관리 센터에서 "지금 정책을 업데이트할 수 없지만 나중에 다시 시도하십시오."라는 오류가 발생하는 경우 PowerShell을 사용하여 모임 정책을 만들거나 수정하는 Teams 좋습니다. 

모임 정책에 대한 자세한 내용은 다음 리소스를 참조하십시오.

- 정책 만들기, 변경 및 정책에 사용자 할당에 대한 자세한 내용은 [Manage meeting policies in Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- PowerShell cmdlet을 사용하여 정책을 변경하기 위해 [PowerShell Teams 참조하세요.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - 모임 정책에 대해 비즈니스용 Skype [PowerShell](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) 모듈을 Teams 합니다. 
    - 자세한 내용은 [*-CsTeamsMeetingPolicy cmdlet 설명서를](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) 검토하세요.

