---
title: 레거시 eDiscovery 도구 사용 중지
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
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798555"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="85585-102">레거시 eDiscovery 도구 사용 중지</span><span class="sxs-lookup"><span data-stu-id="85585-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="85585-103">Microsoft 365 규정 준수 센터의 새 기능과 향상된 eDiscovery 기능으로 인해 다음 레거시 eDiscovery 도구 및 명령줄은 몇 개월 후 사용 중지됩니다.</span><span class="sxs-lookup"><span data-stu-id="85585-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="85585-104">Exchange 관리 센터의 [In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) 및 [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds)</span><span class="sxs-lookup"><span data-stu-id="85585-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="85585-105">eDiscovery 및 In-Place 보류를 지원하는 Exchange Online PowerShell cmdlet을 In-Place 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85585-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="85585-106">이러한 cmdlet은 \*-MailboxSearch cmdlet으로 총체적으로 식별됩니다. 여기에는 다음 cmdlet이 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="85585-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="85585-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="85585-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="85585-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="85585-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="85585-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="85585-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="85585-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="85585-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="85585-111">Exchange Online PowerShell의 [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet</span><span class="sxs-lookup"><span data-stu-id="85585-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="85585-112">Exchange 웹 서비스 API의 다음 작업</span><span class="sxs-lookup"><span data-stu-id="85585-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="85585-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="85585-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="85585-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="85585-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="85585-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="85585-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="85585-116">Advanced eDiscovery v1.0</span><span class="sxs-lookup"><span data-stu-id="85585-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="85585-117">**사용 중지 타임라인**:</span><span class="sxs-lookup"><span data-stu-id="85585-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="85585-118">**2020년 7월 1일** 더 이상 새 검색 및 보류를 만들 수 없지만 기존 검색을 실행, 편집 및 삭제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85585-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="85585-119">Microsoft 지원은 EAC에서 In-Place eDiscovery & 지원하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="85585-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="85585-120">**2020년 10월 1일** In-Place eDiscovery & EAC의 보류 기능은 읽기 전용 모드로 설정되어 기존 검색 및 보류만 제거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85585-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="85585-121">**자세한 내용은 을 참조하세요.**</span><span class="sxs-lookup"><span data-stu-id="85585-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="85585-122">레거시 eDiscovery 검색 및 보류를 Microsoft 365 규정 준수 센터로 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="85585-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="85585-123">eDiscovery 도구의 사용 중지</span><span class="sxs-lookup"><span data-stu-id="85585-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="85585-124">eDiscovery 및 In-Place 보류에 In-Place FAQ</span><span class="sxs-lookup"><span data-stu-id="85585-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



