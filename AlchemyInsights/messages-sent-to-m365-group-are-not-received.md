---
title: Microsoft 365 그룹에 보낸 메시지를 모든 구성원이 수신하지 않음
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: d2f0674f6be135927dc5995575c14f3c2708df49
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806153"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a><span data-ttu-id="a15a2-102">Microsoft 365 그룹에 보낸 메시지를 모든 구성원이 수신하지 않음</span><span class="sxs-lookup"><span data-stu-id="a15a2-102">Messages sent to a Microsoft 365 group are not received by all members</span></span>

<span data-ttu-id="a15a2-103">모든 그룹 구성원이 구독하여 전자 메일을 수신하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="a15a2-103">Make sure that all group members have subscribed to receive the emails.</span></span> <span data-ttu-id="a15a2-104">[Outlook에서 그룹 팔로우하기](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="a15a2-104">See [Follow a group in Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span></span>  

<span data-ttu-id="a15a2-105">그룹 전자 메일을 구독하는 구성원의 메시지 상태를 확인하려면 [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps)에서 다음 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="a15a2-105">To check the message status of members who have subscribed to group emails, run the following command on [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`