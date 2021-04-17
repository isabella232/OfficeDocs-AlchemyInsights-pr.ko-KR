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
# <a name="calendar-permissions"></a>일정 사용 권한

사용자는 웹용 Outlook 또는 다른 클라이언트에서 자신의 일정 권한을 변경할 수 있지만 관리자 권한도 조사해야 할 수 있습니다.  
Exchange PowerShell cmdlet을 사용하면 사용자의 일정에 대한 사용 권한이 표시됩니다.

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

자세한 내용은 다음을 참조하세요.

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

일정 사용 권한은 Outlook 일정 공유에 대한 자세한 내용은 다음 문서를 참조하세요.

- [다른 사람과 Outlook 일정 공유](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [비즈니스용 웹용 Outlook에서 일정 공유](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

일정 사용 권한 문제를 해결하려면 지원 및 복구 도우미 [도구를 사용할 수](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) 있습니다.