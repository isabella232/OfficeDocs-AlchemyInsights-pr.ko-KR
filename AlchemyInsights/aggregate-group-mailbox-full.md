---
title: AggregateGroupMailbox Microsoft 365 그룹으로 보낸 전자 메일에 대해 수신된 전체 NDR
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
ms.openlocfilehash: 9de09ab4cbd2f09648305b11da6273ed990907cf
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/18/2020
ms.locfileid: "49715726"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox Microsoft 365 그룹으로 보낸 전자 메일에 대해 수신된 전체 NDR

다음 EXO 셸 명령을 사용하여 집계 그룹 사서함으로 전송된 전자 메일을 자동으로 삭제하는 Exchange 전송 규칙을 만들 수 있습니다.

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> **-SentTo의** SMTP 주소를 테넌트에 있는 집계 그룹 사서함의 SMTP 주소로 바 대체합니다. 받은 NDR에서 집계 그룹 사서함의 SMTP 주소를 얻을 수 있습니다.



