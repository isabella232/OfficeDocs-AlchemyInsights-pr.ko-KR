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
ms.openlocfilehash: 6655bbe9482400eeb3cfdf0b91bdc595e3d98fbff0f6d9244db8bb4dd958305e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951859"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox Microsoft 365 그룹에 전송된 전자 메일에 대해 수신된 전체 NDR

다음 EXO 셸 명령을 사용하여 집계 그룹 Exchange 전자 메일을 자동으로 삭제하는 exO 전송 규칙을 만들 수 있습니다.

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> **-SentTo의** SMTP 주소를 테넌트에 있는 집계 그룹 사서함의 SMTP 주소로 바 대체합니다. 받은 NDR에서 집계 그룹 사서함의 SMTP 주소를 얻을 수 있습니다.



