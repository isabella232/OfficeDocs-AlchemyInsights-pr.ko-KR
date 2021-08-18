---
title: AggregateGroupMailbox Microsoft 365 그룹에 전송된 전자 메일에 대해 수신된 전체 NDR
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004286"
- "7656"
ms.openlocfilehash: ace8e256e3771f82512abcb9e20b832381eedf80
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315916"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox Microsoft 365 그룹에 전송된 전자 메일에 대해 수신된 전체 NDR

다음 EXO 셸 명령을 사용하여 집계 그룹 Exchange 전자 메일을 자동으로 삭제하는 exO 전송 규칙을 만들 수 있습니다.

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

**참고:** **-SentTo의** SMTP 주소를 테넌트에 있는 집계 그룹 사서함의 SMTP 주소로 바 대체합니다. 받은 NDR에서 집계 그룹 사서함의 SMTP 주소를 얻을 수 있습니다.



