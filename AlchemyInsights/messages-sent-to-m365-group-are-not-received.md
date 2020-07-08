---
title: Microsoft 365 그룹에 보낸 메시지를 모든 구성원이 수신하지 않음
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 2c98841aaa278c1bc18b3ec9007240b1e856f41e
ms.sourcegitcommit: 743a9e4967993c5463272240280c22e27a8dc5b6
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/06/2020
ms.locfileid: "45047236"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Microsoft 365 그룹에 보낸 메시지를 모든 구성원이 수신하지 않음

모든 그룹 구성원이 구독하여 전자 메일을 수신하는지 확인합니다. [Outlook에서 그룹 팔로우하기](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36)를 참조하세요.  

그룹 전자 메일을 구독하는 구성원의 메시지 상태를 확인하려면 [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps)에서 다음 명령을 실행합니다.

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`