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
ms.openlocfilehash: 78ceac80626159e72af5f9ac963365c5c057a4ef0de2b3dc7e4cde5e5cc155e5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068170"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>CompletedWithErrors 상태가 완료된 공용 폴더 마이그레이션 일괄 처리의 경우

다음 단계에 따라 큰/불량 항목을 건너뛰고 일괄 처리를 완료합니다. 
1. 마이그레이션 일괄 처리에서 건너뛴 항목을 승인합니다.

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. 다음 명령을 사용하여 "동기화"되지만 완료되지 않은 마이그레이션 요청에서 건너뛴 항목을 승인합니다.

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. 마이그레이션 일괄 처리 및 요청이 몇 분 후에 다시 시작 및 완료됩니다.

