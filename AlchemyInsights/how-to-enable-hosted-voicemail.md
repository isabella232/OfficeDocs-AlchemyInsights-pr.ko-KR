---
title: 호스트된 음성메일을 사용하도록 설정하는 방법
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 4d70e92a7c1bf8f3cc62d4a310aa140ee2dfdef4c798ae17faa961736d9db500
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055560"
---
# <a name="how-to-enable-hosted-voicemail"></a>호스트된 음성메일을 사용하도록 설정하는 방법

음성메일을 사용하도록 설정하려면 **HostedVoicemail을** 음성으로 $true.

RPS(원격 PowerShell)를 사용하는 사용자의 **HostedVoicemail** 속성

RPS에 연결하는 데 대한 자세한 내용은 Microsoft Teams [PowerShell Overview를](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 참조하세요.

1. 관리자 Teams 대한 원격 PowerShell에 로그인해야 Teams.
1. PowerShell 프롬프트에서 Teams 관리자는 **set-csuser user@contoso.com -HostedVoiceMail** $true sip uri가 해당 사용자의 위치인 set-csuser를 실행할 수 있습니다.

> [!NOTE]
> 정책 변경 내용을 복제하는 데 최대 24시간이 걸릴 수 있습니다.