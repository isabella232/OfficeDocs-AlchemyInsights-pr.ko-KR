---
title: 보낸 사람이 Microsoft 365 그룹으로 보낸 전자 메일을 수신하지 않습니다.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b3b438e17c35f18289d3e9c3ca89d16a6f2a065f
ms.sourcegitcommit: dcca0df53f9194f406cf3a5f6b046cb33a0a5b03
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/21/2020
ms.locfileid: "46846059"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a><span data-ttu-id="7fd43-102">보낸 사람이 Microsoft 365 그룹으로 보낸 전자 메일을 수신하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="7fd43-102">Sender does not receive email sent to Microsoft 365 group</span></span>

<span data-ttu-id="7fd43-103">기본적으로 Microsoft 365 그룹에 전자 메일 메시지를 보낸 사람은 보낸 사람이 그룹의 구성원인 경우에도 받은 편지함에 메시지 사본을 수신하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="7fd43-103">By default, the sender of an email message to a Microsoft 365 group doesn't receive a copy of the message in their Inbox, even if the sender is a member of the group.</span></span>

<span data-ttu-id="7fd43-104">다음 EXO PowerShell 명령을 사용하여 보낸 사람이 Microsoft 365 그룹에 보내는 각 전자 메일의 복사본을 받을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7fd43-104">Use this EXO PowerShell command to allow the sender to receive a copy of each email they send to the Microsoft 365 group:</span></span>  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

<span data-ttu-id="7fd43-105">모든 사서함에 대한 설정을 한 번에 사용하려면 다음을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="7fd43-105">To enable the setting for all mailboxes at once:</span></span>

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

<span data-ttu-id="7fd43-106">**참고** 이 설정의 변경 내용을 적용하려면 최대 1시간이 걸립니다.</span><span class="sxs-lookup"><span data-stu-id="7fd43-106">**Note** Changes to this setting take up to an hour to take effect.</span></span>