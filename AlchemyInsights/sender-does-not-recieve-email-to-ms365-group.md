---
title: 보낸 사람이 Microsoft 365 그룹으로 보낸 전자 메일을 수신하지 않습니다.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b8091305d55408f51cf369506acc7bfac59defb5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751321"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a><span data-ttu-id="48c48-102">보낸 사람이 Microsoft 365 그룹으로 보낸 전자 메일을 수신하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="48c48-102">Sender does not receive email sent to Microsoft 365 group</span></span>

<span data-ttu-id="48c48-103">기본적으로 Microsoft 365 그룹에 전자 메일 메시지를 보낸 사람은 보낸 사람이 그룹의 구성원인 경우에도 받은 편지함에 메시지 사본을 수신하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="48c48-103">By default, the sender of an email message to a Microsoft 365 group doesn't receive a copy of the message in their Inbox, even if the sender is a member of the group.</span></span>

<span data-ttu-id="48c48-104">다음 EXO PowerShell 명령을 사용하여 보낸 사람이 Microsoft 365 그룹에 보내는 각 전자 메일의 복사본을 받을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="48c48-104">Use this EXO PowerShell command to allow the sender to receive a copy of each email they send to the Microsoft 365 group:</span></span>  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

<span data-ttu-id="48c48-105">모든 사서함에 대한 설정을 한 번에 사용하려면 다음을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="48c48-105">To enable the setting for all mailboxes at once:</span></span>

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

<span data-ttu-id="48c48-106">**참고** 이 설정의 변경 내용을 적용하려면 최대 1시간이 걸립니다.</span><span class="sxs-lookup"><span data-stu-id="48c48-106">**Note** Changes to this setting take up to an hour to take effect.</span></span>