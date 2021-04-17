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
ms.openlocfilehash: 07609b39149c003b029f3ea5669f4044af43c25d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826169"
---
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="3a08e-102">PST 가져오기 문제 해결</span><span class="sxs-lookup"><span data-stu-id="3a08e-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="3a08e-103">Outlook 클라이언트 자체 내에서 가져오는 경우, [Outlook .pst 파일을 가져올 때 발생하는 문제 해결](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="3a08e-103">If you are importing within the Outlook client itself, please see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="3a08e-104">가져오기 서비스를 사용하고 멈춤이 발생하는 경우, Azure Storage 위치에 업로드하는 각 PST 파일은 20GB를 초과하지 않아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="3a08e-104">If you are using Import Service and it is stuck, please note that each PST file that you upload to the Azure Storage location should be no larger than 20 GB.</span></span> <span data-ttu-id="3a08e-105">20GB보다 큰 PST 파일은 PST 가져오기 프로세스의 성능에 영향을 줄 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3a08e-105">PST files larger than 20 GB may impact the performance of the PST import process.</span></span>

- <span data-ttu-id="3a08e-106">특정 가져오기 작업의 상태를 확인하려는 경우[Get-MailboxImportRequest-batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest)을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3a08e-106">If you want to verify the status of a specific Import job, you can use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="3a08e-107">가져오기 서비스에 대한 자세한 내용은 [조직의 PST 파일 가져오기에 대한 개요](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="3a08e-107">For full details on the import service, please see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
