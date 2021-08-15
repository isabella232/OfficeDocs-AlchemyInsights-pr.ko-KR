---
title: NDI 기술 켜기
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
- "9004403"
- "7947"
ms.openlocfilehash: ed932592aae1158bc0c0da4817467b69d20208533bc080cb0e424f552af8601a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54023528"
---
# <a name="turn-on-ndi-technology"></a>NDI 기술 켜기

NDI 기술을 사용하려면 사용자에 대해 다음 두 단계를 켜야 합니다.

1. 테넌트 관리자는 CsTeamsMeetingPolicy에서 'AllowNDIStreaming' 속성을 사용하도록 설정해야 합니다.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. 이 변경이 채워진 후 최종 사용자는 사용 권한 에서 특정 클라이언트에 대한 NDI® 기술을 **켜야 설정 > 합니다.**

자세한 내용은 [에서 NDI 기술](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)사용을 Microsoft Teams.
