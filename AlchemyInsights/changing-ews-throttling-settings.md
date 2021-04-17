---
title: EWS 제한 설정 변경
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
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818042"
---
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="ce340-102">EWS 제한 설정 변경</span><span class="sxs-lookup"><span data-stu-id="ce340-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="ce340-103">마이그레이션 기간 동안 EWS 제한 정책을 수정할 수 있도록 해주는 당사의 자동화된 테스트를 실행하세요.</span><span class="sxs-lookup"><span data-stu-id="ce340-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="ce340-104">이 항목이 실행된 후에도 EWS 가져오기는 사서함당 5분당 150mb로 제한됩니다. 더 높은 마이그레이션 처리 속도를 얻으려면 더 많은 사용자를 동시에 마이그레이션하시기 바랍니다.</span><span class="sxs-lookup"><span data-stu-id="ce340-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="ce340-105">EWS 제한 정책의 변경 사항은 다음의 마이그레이션 유형(Microsoft 도구 사용)에 영향을 주지 않는다는 점에 유의하세요: Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder 또는 PST Import Service</span><span class="sxs-lookup"><span data-stu-id="ce340-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>