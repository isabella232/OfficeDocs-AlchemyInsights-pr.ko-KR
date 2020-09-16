---
title: 일정 권한
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: cfee520e26587c0a649c08084853c31232d027f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748799"
---
# <a name="calendar-permissions"></a><span data-ttu-id="5520d-102">일정 권한</span><span class="sxs-lookup"><span data-stu-id="5520d-102">Calendar Permissions</span></span>

<span data-ttu-id="5520d-103">사용자는 웹 이나 다른 클라이언트에서 Outlook을 사용 하 여 자신의 일정 권한을 변경할 수 있으며, 관리자는이를 조사 해야 할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5520d-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="5520d-104">Exchange PowerShell cmdlet을 사용 하면 사용자의 일정에 대 한 사용 권한을 표시 합니다.</span><span class="sxs-lookup"><span data-stu-id="5520d-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="5520d-105">자세한 내용은 다음 항목을 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="5520d-105">To see more information see the following:</span></span>

- [<span data-ttu-id="5520d-106">Get-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="5520d-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="5520d-107">Add-mailboxfolderpermission</span><span class="sxs-lookup"><span data-stu-id="5520d-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="5520d-108">Add-mailboxfolderpermission 추가</span><span class="sxs-lookup"><span data-stu-id="5520d-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="5520d-109">캘린더 사용 권한은 일정을 공유 하는 데 사용 되며, Outlook 일정 공유에 대 한 자세한 내용은 다음 문서를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="5520d-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="5520d-110">다른 사람과 Outlook 일정 공유</span><span class="sxs-lookup"><span data-stu-id="5520d-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="5520d-111">비즈니스용 웹용 Outlook에서 일정 공유</span><span class="sxs-lookup"><span data-stu-id="5520d-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="5520d-112">일정 권한 문제를 해결 하려면 [지원 및 복구 도우미](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) 도구를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5520d-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>