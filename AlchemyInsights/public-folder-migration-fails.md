---
title: 95%에서 공용 폴더 마이그레이션이 실패함
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: fc8da45d91d5c32be52e48770e469cf25eb068f5
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/26/2020
ms.locfileid: "46903592"
---
# <a name="public-folder-migration-fails-at-95"></a><span data-ttu-id="e5ea5-102">95%에서 공용 폴더 마이그레이션이 실패함</span><span class="sxs-lookup"><span data-stu-id="e5ea5-102">Public folder migration fails at 95%</span></span>

<span data-ttu-id="e5ea5-103">FailedToMailEnablePublicFoldersException 오류에 의해 95%에서 실패하는 공용 폴더 마이그레이션:</span><span class="sxs-lookup"><span data-stu-id="e5ea5-103">For public folder migrations failing at 95%, with error FailedToMailEnablePublicFoldersException:</span></span>

1. <span data-ttu-id="e5ea5-104">Exchange 온-프레미스 서버에서 [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) 스크립트를 다운로드하고 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="e5ea5-104">Download and run the [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) script at your Exchange On-Premises server.</span></span>

2. <span data-ttu-id="e5ea5-105">스크립트가 제안한 수정 조치를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="e5ea5-105">Perform the corrective actions suggested by the script.</span></span>

3. <span data-ttu-id="e5ea5-106">Sync-MailPublicFolders(Exchange 2010의 경우) 또는 Sync-ModernMailPublicFolders(Exchange 2013 이상)를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="e5ea5-106">Run the Sync-MailPublicFolders (for Exchange 2010) or Sync-ModernMailPublicFolders (for Exchange 2013 and later).</span></span>

4. <span data-ttu-id="e5ea5-107">공용 폴더 마이그레이션을 다시 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="e5ea5-107">Resume public folder migration.</span></span>
