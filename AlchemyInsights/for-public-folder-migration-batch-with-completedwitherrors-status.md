---
title: CompletedWithErrors 상태인 공용 폴더 마이그레이션 일괄 처리의 경우
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
- "3500007"
- "3532"
ms.openlocfilehash: cbf5237fdb5c660057465e67702e35f68e545ddb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744119"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="695d8-102">CompletedWithErrors 상태인 공용 폴더 마이그레이션 일괄 처리의 경우</span><span class="sxs-lookup"><span data-stu-id="695d8-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="695d8-103">다음 단계에 따라 큰/잘못 된 항목을 건너뛰어 일괄 처리를 완료 합니다.</span><span class="sxs-lookup"><span data-stu-id="695d8-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="695d8-104">마이그레이션 일괄 처리에서 건너뛴 항목을 승인 합니다.</span><span class="sxs-lookup"><span data-stu-id="695d8-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="695d8-105">다음 명령을 사용 하 여 "동기화" 되었지만 완료 되지 않은 마이그레이션 요청에 대해 건너뛴 항목을 승인 합니다.</span><span class="sxs-lookup"><span data-stu-id="695d8-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="695d8-106">마이그레이션 일괄 처리 및 요청이 몇 분 후에 다시 시작 되 고 완료 되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="695d8-106">The migration batch and requests should resume and complete in a few minutes.</span></span>

