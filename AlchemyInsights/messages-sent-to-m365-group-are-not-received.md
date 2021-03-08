---
title: Microsoft 365 그룹에 보낸 메시지를 모든 구성원이 수신하지 않음
ms.author: pebaum
author: pebaum
manager: mnirkhe
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 080c060f5675065704c7209bd15e4cbb1236b8db
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50480689"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Microsoft 365 그룹에 보낸 메시지를 모든 구성원이 수신하지 않음

모든 그룹 구성원이 구독하여 전자 메일을 수신하는지 확인합니다. [Outlook에서 그룹 팔로우하기](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36)를 참조하세요.  

그룹 전자 메일을 구독하는 구성원의 메시지 상태를 확인하려면 [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)에서 다음 명령을 실행합니다.

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

다음 EXO PowerShell 명령을 사용하여 모든 그룹 구성원이 받은 편지함에 Microsoft 365 그룹으로 보낸 전자 메일을 수신하도록 구성합니다.

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

예를 들면 다음과 같습니다.

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`