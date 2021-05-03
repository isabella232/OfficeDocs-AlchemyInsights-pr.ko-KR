---
title: PST 가져오기 문제 해결
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 5065b9895954371e4298c98e8aadb67ba8f140fd
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52059821"
---
# <a name="troubleshooting-pst-import-issues"></a>PST 가져오기 문제 해결

- Outlook 클라이언트 자체 안에서 가져오는 경우, [Outlook.pst 파일을 가져올 때 발생하는 문제 해결](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)을 참조하세요.

- 가져오기 서비스를 사용하고 멈춤이 발생하는 경우, Azure Storage 위치에 업로드하는 각 PST 파일은 20GB를 초과하지 않아야 합니다. 20GB보다 큰 PST 파일은 PST 가져오기 프로세스의 성능에 영향을 줄 수 있습니다. 작업이 멈추는 문제 해결에 대한 자세한 내용은 [PST 가져오기 작업에 영향을 주는 문제](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)를 참조하세요.

- 특정 가져오기 작업의 상태를 확인하려는 경우[Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest)을 사용할 수 있습니다.

- 가져오기 서비스에 대한 자세한 내용은 [조직의 PST 파일 가져오기에 대한 개요](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)를 참조하세요.
