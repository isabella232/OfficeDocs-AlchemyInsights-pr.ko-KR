---
title: 공용 폴더 마이그레이션 일괄 처리 완료되지 않음, 동기화됨 표시
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: 33302110249b02aef87639792ebfd9cafd6638c0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771489"
---
# <a name="public-folder-migration-batch-not-completing-shows-synced"></a><span data-ttu-id="69b89-102">공용 폴더 마이그레이션 일괄 처리 완료되지 않음, 동기화됨 표시</span><span class="sxs-lookup"><span data-stu-id="69b89-102">Public folder migration batch not completing, shows synced</span></span>

<span data-ttu-id="69b89-103">마이그레이션 일괄 처리 완료를 시작했을 수 있습니다. 마이그레이션 일괄 처리의 상태가 오랫동안 “동기화” 상태로 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="69b89-103">You may have initiated completion of migration batch and status of the migration batch continues showing "Synced" for very long time.</span></span> <span data-ttu-id="69b89-104">이는 정상적인 동작입니다.</span><span class="sxs-lookup"><span data-stu-id="69b89-104">This is expected behavior.</span></span>

<span data-ttu-id="69b89-105">일반적으로 마이그레이션 일괄 처리의 상태가 완료로 전환되기 전에 몇 시간 동안 동기화 상태로 남아있습니다.</span><span class="sxs-lookup"><span data-stu-id="69b89-105">It's common for the status of migration batch to remain on Synced for a few hours before it switches to Completing.</span></span> <span data-ttu-id="69b89-106">다수의 대상 사서함이 포함된 마이그레이션의 경우 기본 공용 폴더 마이그레이션 요청이 실패하거나 격리되지 않은 경우 마이그레이션 일괄 처리의 상태는 일반적으로 24시간 이상 동기화 상태로 남아있습니다.</span><span class="sxs-lookup"><span data-stu-id="69b89-106">For migrations involving a large number of target mailboxes, it's normal to see the status remain in the Synced state for more than 24 hours, provided none of the underlying public folder migration requests have failed or were quarantined.</span></span> <span data-ttu-id="69b89-107">마이그레이션 일괄 처리가 완료될 때까지 24~48시간 기다리세요.</span><span class="sxs-lookup"><span data-stu-id="69b89-107">Please allow 24-48 hours for the migration batch to complete the tasks.</span></span>
