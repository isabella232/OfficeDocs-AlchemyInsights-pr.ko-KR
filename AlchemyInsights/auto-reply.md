---
title: Microsoft 365 그룹에 보낸 모든 전자 메일에 대한 자동 응답을 구성하려면 다음과 같이 하세요.
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8586"
- "9003200"
ms.openlocfilehash: 1adc3c131daedb26d88710f4b4078b0622ad13c5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331537"
---
# <a name="to-configure-auto-reply-for-all-emails-sent-to-microsoft-365-group"></a>Microsoft 365 그룹에 보낸 모든 전자 메일에 대한 자동 응답을 구성하려면 다음과 같이 하세요.

**테넌트 관리자 계정을 사용하여 EXO PowerShell에 연결하고 다음 명령어를 사용합니다**.

`Set-MailboxAutoReplyConfiguration -Identity groupmailbox -AutoReplyState Enabled -InternalMessage "Internal auto-reply message." -ExternalMessage "External auto-reply message`

**참고**: **groupmailbox** 를 구성할 그룹 이름으로 변경합니다.

