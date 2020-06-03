---
title: 사서함 감사 사용
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 2bcfb7cc174cd58b21e1bb0c82f0d7cdb25e2fdd
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506960"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="e534a-102">사서함 감사 사용</span><span class="sxs-lookup"><span data-stu-id="e534a-102">Enable mailbox auditing</span></span>

<span data-ttu-id="e534a-103">단일 사용자 또는 전체 조직에 대해 사서함 감사를 사용 하도록 설정 하려면 원격 전원 셸에서 다음 cmdlet을 실행 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="e534a-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="e534a-104">**단일 사용자**</span><span class="sxs-lookup"><span data-stu-id="e534a-104">**Single User**</span></span>
  
<span data-ttu-id="e534a-105">Set-Mailbox-Id "Jane Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="e534a-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="e534a-106">**조직**</span><span class="sxs-lookup"><span data-stu-id="e534a-106">**Organization**</span></span>
  
<span data-ttu-id="e534a-107">Get-Mailbox-ResultSize 무제한-필터 {RecipientTypeDetails-eq "UserMailbox"} | Set-Mailbox-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="e534a-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="e534a-108">자세한 정보</span><span class="sxs-lookup"><span data-stu-id="e534a-108">Learn more</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

