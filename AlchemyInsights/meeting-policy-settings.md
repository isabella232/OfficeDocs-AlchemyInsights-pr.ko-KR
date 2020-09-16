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
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794340"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Microsoft 팀에서 모임 정책 관리

**참고: 정책 변경 내용이 적용 되는 데 최대 24 시간이 걸릴 수 있습니다.** 새로 만든 정책을 즉시 변경 하지 못할 수 있습니다. 4 시간을 기다린 후 새로 만든 정책을 다시 수정 해 보십시오.

모임 정책은 조직의 사용자가 예약한 모임에 대해 모임 참가자가 사용할 수 있는 기능을 제어 하는 데 사용 됩니다. 모임 정책의 일부 기능은 아직 팀 관리 센터에서 구현 되지 않을 수 있습니다 (설명서에서 "출시 예정" 라는 레이블이 지정 되어 있음). 이 경우 또는 "지금은 정책을 업데이트할 수 없지만 나중에 다시 시도 합니다."와 같은 오류가 나타나면 PowerShell을 사용 하 여 팀 회의 정책을 만들거나 수정 하는 것이 좋습니다. 

모임 정책에 대 한 자세한 내용은 다음 리소스를 참조 하십시오.

- 정책을 만들고, 변경 하 고, 사용자를 정책에 할당 하는 방법에 대 한 자세한 내용은 [팀에서 모임 정책 관리](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)를 참조 하십시오.

- PowerShell cmdlet을 사용 하 여 정책을 변경 하려면 [팀 Powershell 개요](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)를 참조 하세요. 
    - 팀 회의 정책에 [비즈니스용 Skype PowerShell 모듈](https://www.microsoft.com/download/details.aspx?id=39366) 을 사용 해야 합니다. 
    - 자세한 내용은 [*-CsTeamsMeetingPolicy cmdlet 설명서](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) 를 참조 하십시오.

