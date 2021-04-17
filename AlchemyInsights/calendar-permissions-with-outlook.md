---
title: 일정 사용 권한
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: bbd49134bd4a4451649b76bb5f60b19065910cae
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819914"
---
# <a name="calendar-permissions"></a><span data-ttu-id="8a787-102">일정 사용 권한</span><span class="sxs-lookup"><span data-stu-id="8a787-102">Calendar Permissions</span></span>

<span data-ttu-id="8a787-103">사용자는 웹용 Outlook 또는 다른 클라이언트에서 자신의 일정 권한을 변경할 수 있지만 관리자 권한도 조사해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8a787-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="8a787-104">Exchange PowerShell cmdlet을 사용하면 사용자의 일정에 대한 사용 권한이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="8a787-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="8a787-105">자세한 내용은 다음을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="8a787-105">To see more information see the following:</span></span>

- [<span data-ttu-id="8a787-106">Get-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="8a787-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="8a787-107">Set-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="8a787-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="8a787-108">Add-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="8a787-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="8a787-109">일정 사용 권한은 Outlook 일정 공유에 대한 자세한 내용은 다음 문서를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="8a787-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="8a787-110">다른 사람과 Outlook 일정 공유</span><span class="sxs-lookup"><span data-stu-id="8a787-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="8a787-111">비즈니스용 웹용 Outlook에서 일정 공유</span><span class="sxs-lookup"><span data-stu-id="8a787-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="8a787-112">일정 사용 권한 문제를 해결하려면 지원 및 복구 도우미 [도구를 사용할 수](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8a787-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>