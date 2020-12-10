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
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49608847"
---
# <a name="how-to-enable-hosted-voicemail"></a>호스트된 음성메일을 사용하도록 설정하는 방법

음성메일을 사용하도록 설정하려면 **HostedVoicemail을** 음성 $true.

RPS(원격 PowerShell)를 사용하는 사용자의 **HostedVoicemail** 속성입니다.

RPS에 연결하는 데 대한 자세한 내용은 RPS에 연결하는 데 대한 자세한 내용은 [Microsoft Teams PowerShell 개요를](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 참조하세요.

1. Teams 관리자는 Teams용 원격 PowerShell에 로그인해야 합니다.
1. PowerShell 프롬프트에서 Teams 관리자는 **set-csuser user@contoso.com -HostedVoiceMail** $true sip uri가 해당 사용자의 위치인 set-csuser를 실행할 수 있습니다.

> [!NOTE]
> 정책 변경 내용을 복제하는 데 최대 24시간이 걸릴 수 있습니다.