---
title: Office 365 그룹 또는 팀을 주소 목록에서 숨기기 또는 숨기기 취소
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: 1204b9f45fe34015f72c559f77674e980d28c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47782333"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a><span data-ttu-id="7f38f-102">Office 365 그룹 또는 팀을 주소 목록에서 숨기기 또는 숨기기 취소</span><span class="sxs-lookup"><span data-stu-id="7f38f-102">Hide or un-hide Office 365 groups or teams from address list</span></span>

<span data-ttu-id="7f38f-103">다음 EXO PowerShell 명령을 사용하여 Exchange 클라이언트(Outlook, OWA)의 주소 목록(GAL)에서 Office 365 그룹/팀을 숨기거나 숨기기 취소할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7f38f-103">Use the following EXO PowerShell command to hide or un-hide Office 365 group/teams from address lists (GAL) of Exchange clients (Outlook, OWA):</span></span>

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

<span data-ttu-id="7f38f-104">다음 EXO PowerShell 명령을 사용하여 Exchange 클라이언트(Outlook, OWA)에서 Office 365 그룹/팀을 숨기거나 숨기기 취소할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7f38f-104">Use the following EXO PowerShell command to hide or un-hide the Office365 group/teams from Exchange clients (Outlook, OWA):</span></span>

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- <span data-ttu-id="7f38f-105">자세한 지침은 [GAL 및 Exchange 클라이언트에서 Office 365 그룹 숨기기](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="7f38f-105">For detailed instructions, see [Hide Office 365 Groups from the GAL and Exchange Clients](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).</span></span>
