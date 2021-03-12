---
title: 모임 정책 설정
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
- "9000734"
- "2657"
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704612"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Microsoft Teams에서 모임 정책 관리

**참고: 정책 변경 내용이 사용자에게 적용될 경우 최대 24시간이 걸릴 수 있습니다.** 새로 만든 정책을 즉시 변경하지 못하게 될 수 있습니다. 4시간을 기다렸다가 새로 만든 정책을 다시 수정하려고 합니다.

모임 정책은 조직의 사용자가 예약한 모임에 대해 모임 참가자가 사용할 수 있는 기능을 제어하는 데 사용됩니다. 모임 정책의 일부 기능은 아직 Teams 관리 센터에서 구현되지 않을 수 있습니다(설명서에서 "곧 제공될 예정"으로 레이블이 지정되어 있습니다). 이 경우 또는 Microsoft Teams 관리 센터에서 "지금 정책을 업데이트할 수 없지만 나중에 다시 시도하십시오."라는 오류가 발생하는 경우 PowerShell을 사용하여 Teams 모임 정책을 만들거나 수정하는 것이 좋습니다. 

모임 정책에 대한 자세한 내용은 다음 리소스를 참조하십시오.

- 정책을 만들고, 변경하고, 사용자를 정책에 할당하는 방법을 알아보는 자세한 내용은 Teams에서 모임 정책 [관리를 참조합니다.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- PowerShell cmdlet을 사용하여 정책을 변경하기 위해 [Teams PowerShell 개요를 참조하세요.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Teams 모임 정책에 [비즈니스용 Skype PowerShell](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) 모듈을 사용해야 합니다. 
    - 자세한 내용은 [*-CsTeamsMeetingPolicy cmdlet 설명서를](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) 검토하세요.

