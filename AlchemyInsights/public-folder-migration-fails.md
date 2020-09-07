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
ms.openlocfilehash: c1c4210baf93f0071a12f1902fb5f6fbf7bd0716
ms.sourcegitcommit: d3ace2376195d54229ee1e232daf8133ba4e58a9
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/03/2020
ms.locfileid: "47341387"
---
# <a name="public-folder-migration-fails-at-95"></a><span data-ttu-id="5d6ce-102">95%에서 공용 폴더 마이그레이션이 실패함</span><span class="sxs-lookup"><span data-stu-id="5d6ce-102">Public folder migration fails at 95%</span></span>

<span data-ttu-id="5d6ce-103">마이그레이션 일괄 처리 완료를 시작했을 수 있습니다. 마이그레이션 일괄 처리의 상태가 오랜 기간 **동기화** 상태로 계속 표시되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="5d6ce-103">You might have initiated completion of a migration batch, and the status of the migration batch continues showing **Synced** for a very long time.</span></span> <span data-ttu-id="5d6ce-104">이는 정상적인 동작입니다.</span><span class="sxs-lookup"><span data-stu-id="5d6ce-104">This is expected behavior.</span></span>

<span data-ttu-id="5d6ce-105">일반적으로 마이그레이션 일괄 처리의 상태가 **완료**로 전환되기 전에 몇 시간 동안 **동기화** 상태로 남아있습니다.</span><span class="sxs-lookup"><span data-stu-id="5d6ce-105">It's common for the status of a migration batch to remain on **Synced** for a few hours before it switches to **Completing**.</span></span> <span data-ttu-id="5d6ce-106">다수의 대상 사서함이 포함된 마이그레이션의 경우 기본 공용 폴더 마이그레이션 요청이 실패하거나 격리되지 않은 경우 마이그레이션 일괄 처리의 상태는 일반적으로 24시간 이상 동기화 상태로 남아있습니다.</span><span class="sxs-lookup"><span data-stu-id="5d6ce-106">For migrations involving a large number of target mailboxes, it's normal to see the status remain in the synced state for more than 24 hours, provided none of the underlying public folder migration requests have failed or were quarantined.</span></span> <span data-ttu-id="5d6ce-107">마이그레이션 일괄 처리가 완료될 때까지 24~48시간 기다리세요.</span><span class="sxs-lookup"><span data-stu-id="5d6ce-107">Please allow 24-48 hours for the migration batch to complete the tasks.</span></span>

<span data-ttu-id="5d6ce-108">FailedToMailEnablePublicFoldersException 오류에 의해 95%에서 실패하는 공용 폴더 마이그레이션:</span><span class="sxs-lookup"><span data-stu-id="5d6ce-108">For public folder migrations failing at 95%, with error FailedToMailEnablePublicFoldersException:</span></span>

1. <span data-ttu-id="5d6ce-109">Exchange 온-프레미스 서버에서 [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) 스크립트를 다운로드하고 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="5d6ce-109">Download and run the [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) script at your Exchange On-Premises server.</span></span>

2. <span data-ttu-id="5d6ce-110">스크립트가 제안한 수정 조치를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="5d6ce-110">Perform the corrective actions suggested by the script.</span></span>

3. <span data-ttu-id="5d6ce-111">Sync-MailPublicFolders(Exchange 2010의 경우) 또는 Sync-ModernMailPublicFolders(Exchange 2013 이상)를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="5d6ce-111">Run the Sync-MailPublicFolders (for Exchange 2010) or Sync-ModernMailPublicFolders (for Exchange 2013 and later).</span></span>

4. <span data-ttu-id="5d6ce-112">공용 폴더 마이그레이션을 다시 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="5d6ce-112">Resume public folder migration.</span></span>
