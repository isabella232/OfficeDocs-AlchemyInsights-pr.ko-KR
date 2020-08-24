---
title: Microsoft 365 그룹으로 보내기
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: cfb4bd5ce59eeccdd0812d013b8a444aebeb1d4c
ms.sourcegitcommit: 9818d3c8e6b10f23244e51286e2463caf48fffd5
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/21/2020
ms.locfileid: "46853009"
---
# <a name="send-as-microsoft-365-group"></a><span data-ttu-id="52d73-102">Microsoft 365 그룹으로 보내기</span><span class="sxs-lookup"><span data-stu-id="52d73-102">Send As Microsoft 365 group</span></span>

<span data-ttu-id="52d73-103">특정 사용자가 Microsoft 365 그룹으로 메시지를 보낼 수 있도록 다른 사람 이름으로 보내기 권한을 할당할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="52d73-103">You can assign Send As permissions to allow specific users to send messages as a Microsoft 365 group:</span></span>  

1. <span data-ttu-id="52d73-104">Exchange Online PowerShell에 연결합니다.</span><span class="sxs-lookup"><span data-stu-id="52d73-104">Connect to Exchange Online PowerShell.</span></span>  

2. <span data-ttu-id="52d73-105">다음 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="52d73-105">Run the following command:</span></span>  

    <span data-ttu-id="52d73-106">Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs</span><span class="sxs-lookup"><span data-stu-id="52d73-106">Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs</span></span>

<span data-ttu-id="52d73-107">자세한 내용은 [그룹을 사용하여 다른 이름으로 보내거나 그룹을 대신하여 보내기](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="52d73-107">For more information, see [Allow members to send as or send on behalf of a group](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).</span></span>