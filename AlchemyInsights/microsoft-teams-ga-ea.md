---
title: Microsoft Teams - 게스트 액세스
ms.author: heidip
author: microsoftheidi
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "311"
- "6500001"
ms.openlocfilehash: 2c78fec14d43c5cbf6aebbc889d606eb2f6c4c64af85997f523d06872c911a0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012314"
---
# <a name="microsoft-teams---guest-access"></a>Microsoft Teams - 게스트 액세스

조직 외부의 사용자와 통신하는 데 도움이 필요한 Teams 게스트 액세스 또는 [](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access)외부 액세스(페더링)를 사용할지 또는 둘 다 사용할 수 있는지 결정해야 합니다.

차이점을 [검토하여](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access) 각각에 사용할 수 있는 기능을 이해해야 합니다.  예를 들어 외부 액세스(페더ation)를 사용하면 채팅 및 현재 상태와 같은 1:1 통신을 허용합니다.  페더레이션 사용자는 페더레이션 공동 작업에 Teams 수 없습니다.  외부 사용자가 채널 대화 또는 파일 공유를 Teams 참가하려면 게스트 액세스를 설정해야 합니다.

**옵션 1: 게스트 액세스 켜기** Teams 관리 센터에서 [Org Wide 설정 > 게스트](https://admin.teams.microsoft.com/company-wide-settings/guest-configuration) 액세스로 이동한 후 "게스트 액세스 허용"을 Teams.  다른 모든 기본 설정이 있는 테넌트의 경우 이 작업을 모두 해야 합니다.  게스트 액세스 구성을 사용자 지정하려면 게스트 액세스 검사 목록의 모든 단계를 [따라야 합니다.](https://docs.microsoft.com/microsoftteams/guest-access-checklist) 완전히 완료되면 설정이 적용될 때까지 [최대 24시간을](https://docs.microsoft.com/microsoftteams/manage-guests#guest-access-latencies) 기다려야 합니다.

검사 목록의 모든 단계를 완료했다고 확신할 수 있으며 24시간이 지난 경우 진행하여 팀에 게스트를 [추가해 하세요.](https://support.office.com/article/add-guests-to-a-team-in-teams-fccb4fa6-f864-4508-bdde-256e7384a14f#ID0EAABAAA=Desktop)

방법 비디오를 비롯한 자세한 내용은 에서 게스트 액세스를 [Microsoft Teams.](https://docs.microsoft.com/microsoftteams/guest-access)

**옵션 2: 외부 액세스 켜기(페더전)** 또한 외부 액세스(페더ation)를 켜고자 하는 경우 Teams 관리 센터에서 조직 전체 설정 > [외부](https://admin.teams.microsoft.com/company-wide-settings/external-communications) 액세스로 이동하여 "사용자가 비즈니스용 Skype 및 Teams 사용자와 통신할 수 있습니다."를 켜고 Teams 사용자가 다른 조직의 사용자와 채팅하고 통신할 수 있도록 허용의 [모든](https://docs.microsoft.com/microsoftteams/manage-external-access#let-your-teams-users-chat-and-communicate-with-users-in-another-organization)단계를 수행합니다.
