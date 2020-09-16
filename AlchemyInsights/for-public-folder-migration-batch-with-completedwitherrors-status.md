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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>CompletedWithErrors 상태인 공용 폴더 마이그레이션 일괄 처리의 경우

다음 단계에 따라 큰/잘못 된 항목을 건너뛰어 일괄 처리를 완료 합니다. 
1. 마이그레이션 일괄 처리에서 건너뛴 항목을 승인 합니다.

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. 다음 명령을 사용 하 여 "동기화" 되었지만 완료 되지 않은 마이그레이션 요청에 대해 건너뛴 항목을 승인 합니다.

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. 마이그레이션 일괄 처리 및 요청이 몇 분 후에 다시 시작 되 고 완료 되어야 합니다.

