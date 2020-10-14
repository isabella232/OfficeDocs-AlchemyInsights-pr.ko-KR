---
title: Microsoft 팀-게스트 액세스
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
ms.openlocfilehash: ee38dcb5f40ea16cea1b84b9b16e86b0f52f2d89
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/13/2020
ms.locfileid: "48452234"
---
# <a name="microsoft-teams---guest-access"></a>Microsoft 팀-게스트 액세스

팀에서 조직 외부의 사용자와 통신 하는 데 도움이 필요한 경우에는 [게스트 액세스 또는 페더레이션 (외부 액세스)](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access)을 사용할지 또는 두 가지를 모두 사용할 수 있는지를 결정 해야 합니다.

[차이점을 검토](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access) 하 여 각각에 대해 사용할 수 있는 기능을 파악 해야 합니다.  예를 들어 페더레이션 (외부 액세스)은 채팅 및 현재 상태와 같은 1:1 통신을 허용 합니다.  그러나 페더레이션 사용자는 팀 공동 작업에 참여할 수 없습니다.  외부 사용자가 참가 하 고 팀 채널 대화에 참여 하 고 파일을 공유 하려는 경우에는 게스트 액세스를 설정 해야 합니다.

**옵션 1: 게스트 액세스 설정** 팀 관리 센터에서 [조직 수준 설정 > 게스트 액세스 권한](https://admin.teams.microsoft.com/company-wide-settings/guest-configuration) 으로 이동 하 여 "팀에서 게스트 액세스 허용"을 켜십시오.  다른 모든 기본 설정이 포함 된 테 넌 트의 경우에는이 작업을 수행 해야 합니다.  게스트 액세스 구성을 사용자 지정 하려면 [게스트 액세스 검사 목록의](https://docs.microsoft.com/microsoftteams/guest-access-checklist)모든 단계를 수행 해야 합니다. 작업을 완료 한 후에는 [24 시간까지 기다린](https://docs.microsoft.com/microsoftteams/manage-guests#guest-access-latencies) 후 설정을 적용 해야 합니다.

검사 목록의 모든 단계를 완료 했 고 24 시간이 지난 것으로 확신 하는 경우에는 [팀에 게스트를 추가](https://support.office.com/article/add-guests-to-a-team-in-teams-fccb4fa6-f864-4508-bdde-256e7384a14f#ID0EAABAAA=Desktop)해 봅니다.

방법 비디오를 비롯 한 자세한 내용은 [Microsoft 팀의 게스트 액세스](https://docs.microsoft.com/microsoftteams/guest-access)를 참조 하세요.

**옵션 2: 외부 액세스 (페더레이션) 설정** 외부 액세스 (페더레이션)를 설정 하려는 경우에는 팀 관리 센터에서 [외부 액세스 > 조직 전체 설정](https://admin.teams.microsoft.com/company-wide-settings/external-communications) 으로 이동 하 여 "사용자가 비즈니스용 Skype 및 팀 사용자와 통신할 수 있습니다."를 설정한 다음, [팀에서 다른 조직의 사용자와 채팅 하 고 통신](https://docs.microsoft.com/microsoftteams/manage-external-access#let-your-teams-users-chat-and-communicate-with-users-in-another-organization)하는 데 사용 하는 모든 단계를 수행 합니다.
