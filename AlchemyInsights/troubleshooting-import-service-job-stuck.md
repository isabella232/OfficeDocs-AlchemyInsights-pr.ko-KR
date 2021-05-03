---
title: 가져오기 서비스 작업 멈춤 문제 해결
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52059847"
---
# <a name="troubleshooting-import-service-job-stuck"></a><span data-ttu-id="054ec-102">가져오기 서비스 작업 멈춤 문제 해결</span><span class="sxs-lookup"><span data-stu-id="054ec-102">Troubleshooting Import Service job stuck</span></span>

<span data-ttu-id="054ec-103">가져오기 서비스 작업이 멈추거나 실패한 경우 다음을 검토하고 시도합니다.</span><span class="sxs-lookup"><span data-stu-id="054ec-103">If you are experiencing issues with Import service jobs stuck or failing, examine and try the following:</span></span>

- <span data-ttu-id="054ec-104">PST 파일의 크기를 검토합니다.</span><span class="sxs-lookup"><span data-stu-id="054ec-104">Review the size of of the PST file.</span></span> <span data-ttu-id="054ec-105">가져오는 PST 파일의 최대 권장 크기는 20GB입니다.</span><span class="sxs-lookup"><span data-stu-id="054ec-105">The maximum recommended size of a PST file for import is 20GB.</span></span>

- <span data-ttu-id="054ec-106">손상으로 인해 건너뛴 항목이 의심되는 경우 Scanpst.exe를 실행하여 PST 파일의 오류를 진단하고 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="054ec-106">If you suspect skipped items due to corruption, run Scanpst.exe to diagnose and fix errors in PST files.</span></span>

- <span data-ttu-id="054ec-107">가져오는 동안 "MapiExceptionShutoffQuotaExceeded" 오류가 표시되는 경우 대상 사서함에 원하는 PST 파일을 가져오는 데 필요한 용량이 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="054ec-107">If you see a "MapiExceptionShutoffQuotaExceeded" error during import, make sure the target mailbox has sufficient capacity to import the desired PST files.</span></span>

<span data-ttu-id="054ec-108">PST 가져오기 작업 문제 해결에 대한 자세한 내용은 [PST 가져오기 작업 문제 해결](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="054ec-108">For more information on troubleshooting PST import job issues, see [Troubleshoot issues with PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

<span data-ttu-id="054ec-109">Outlook으로 PST를 가져올 때 문제를 해결하는 방법에 대한 자세한 내용은 [Outlook .pst 파일을 가져올 때 발생하는 문제 해결(microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="054ec-109">For information about how to fix issues when importing PSTs into Outlook, see [Fix problems importing an Outlook .pst file (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span></span>