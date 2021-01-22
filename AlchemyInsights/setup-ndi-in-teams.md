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
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/21/2021
ms.locfileid: "49917315"
---
# <a name="turn-on-ndi-technology"></a>NDI 기술 켜기

NDI 기술을 사용하려면 사용자에게 다음 두 단계를 설정해야 합니다.

1. 테넌트 관리자는 CsTeamsMeetingPolicy에서 'AllowNDIStreaming' 속성을 사용하도록 설정해야 합니다.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. 이 변경이 채워진 후 최종 사용자는 설정 ® 사용 권한에서 특정 클라이언트에 대한 NDI® 기술을 **> 켜야 합니다.**

자세한 내용은 [Microsoft Teams에서 NDI 기술 사용을 참조하세요.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)
