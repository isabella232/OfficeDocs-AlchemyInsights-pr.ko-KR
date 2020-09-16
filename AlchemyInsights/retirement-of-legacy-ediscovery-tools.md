---
title: 레거시 eDiscovery 도구 만료
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
- "9001487"
- "3523"
ms.openlocfilehash: 2315c4c651a83f0ecc78c0171f32aba13bc93f8c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727789"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="c3b47-102">레거시 eDiscovery 도구 만료</span><span class="sxs-lookup"><span data-stu-id="c3b47-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="c3b47-103">Microsoft 365 준수 센터에서 새롭게 향상 된 eDiscovery 기능을 사용 하는 경우 다음과 같은 레거시 eDiscovery 도구 및 commandlets이 제공 되는 달에 폐기 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c3b47-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="c3b47-104">Exchange 관리 센터의 원본 [위치 eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) 및 [현재 위치 유지](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds)</span><span class="sxs-lookup"><span data-stu-id="c3b47-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="c3b47-105">원본 위치 eDiscovery 및 원본 위치 유지를 지 원하는 Exchange Online PowerShell cmdlet입니다.</span><span class="sxs-lookup"><span data-stu-id="c3b47-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="c3b47-106">(이러한 cmdlet은 집합적으로 \*-New-mailboxsearch cmdlet으로 식별 됩니다.) 여기에는 다음 cmdlet이 포함 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c3b47-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="c3b47-107">New-mailboxsearch</span><span class="sxs-lookup"><span data-stu-id="c3b47-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="c3b47-108">시작-New-mailboxsearch</span><span class="sxs-lookup"><span data-stu-id="c3b47-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="c3b47-109">New-mailboxsearch</span><span class="sxs-lookup"><span data-stu-id="c3b47-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="c3b47-110">New-mailboxsearch</span><span class="sxs-lookup"><span data-stu-id="c3b47-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="c3b47-111">Exchange Online PowerShell의 [검색 사서함](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet</span><span class="sxs-lookup"><span data-stu-id="c3b47-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="c3b47-112">Exchange 웹 서비스 API에서 다음 작업을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="c3b47-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="c3b47-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="c3b47-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="c3b47-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="c3b47-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="c3b47-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="c3b47-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="c3b47-116">Advanced eDiscovery v 1.0</span><span class="sxs-lookup"><span data-stu-id="c3b47-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="c3b47-117">**만료 시간**:</span><span class="sxs-lookup"><span data-stu-id="c3b47-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="c3b47-118">**2020 년 7 월 1 일** 더 이상 새 검색 및 보류를 만들 수 없지만 기존 검색을 실행, 편집 및 삭제 하는 것은 위험 합니다.</span><span class="sxs-lookup"><span data-stu-id="c3b47-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="c3b47-119">Microsoft Support는 EAC에서 원본 위치 eDiscovery & 보류를 더 이상 지원 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="c3b47-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="c3b47-120">**2020 년 10 월 1 일** 원본 위치 eDiscovery & EAC에서 유지 되는 기능은 읽기 전용 모드로 설정 되므로 기존 검색 및 보류만 제거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c3b47-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="c3b47-121">**자세한 내용은 다음 항목을 참조**하십시오.</span><span class="sxs-lookup"><span data-stu-id="c3b47-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="c3b47-122">레거시 eDiscovery 검색 및 보류를 Microsoft 365 준수 센터로 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="c3b47-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="c3b47-123">eDiscovery 도구의 사용 중지</span><span class="sxs-lookup"><span data-stu-id="c3b47-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="c3b47-124">원본 위치 eDiscovery 및 현재 위치 유지 관련 Faq</span><span class="sxs-lookup"><span data-stu-id="c3b47-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



