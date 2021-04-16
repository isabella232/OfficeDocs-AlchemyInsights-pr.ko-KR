---
title: CompletedWithErrors 상태가 완료된 공용 폴더 마이그레이션 일괄 처리의 경우
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
- "3500007"
- "3532"
ms.openlocfilehash: 9ed21bfb9069b56a4fc59b201bb3ad94c6bb6712
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812470"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="25347-102">CompletedWithErrors 상태가 완료된 공용 폴더 마이그레이션 일괄 처리의 경우</span><span class="sxs-lookup"><span data-stu-id="25347-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="25347-103">다음 단계에 따라 큰/불량 항목을 건너뛰고 일괄 처리를 완료합니다.</span><span class="sxs-lookup"><span data-stu-id="25347-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="25347-104">마이그레이션 일괄 처리에서 건너뛴 항목을 승인합니다.</span><span class="sxs-lookup"><span data-stu-id="25347-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="25347-105">다음 명령을 사용하여 "동기화"되지만 완료되지 않은 마이그레이션 요청에서 건너뛴 항목을 승인합니다.</span><span class="sxs-lookup"><span data-stu-id="25347-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="25347-106">마이그레이션 일괄 처리 및 요청이 몇 분 후에 다시 시작 및 완료됩니다.</span><span class="sxs-lookup"><span data-stu-id="25347-106">The migration batch and requests should resume and complete in a few minutes.</span></span>

