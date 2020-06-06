---
title: 주소 목록에서 그룹을 숨기 거 나 숨기기 취소 하기 위한 지침
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 02368d6a06df90d76ee1bd5448819e7ffe12c18c
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580015"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a><span data-ttu-id="4fe4b-102">주소 목록 (GAL)에서 Microsoft 365 그룹 숨기기</span><span class="sxs-lookup"><span data-stu-id="4fe4b-102">Hide Microsoft 365 group from address list (GAL)</span></span>

<span data-ttu-id="4fe4b-103">Outlook 또는 OWA와 같은 Exchange 클라이언트의 주소 목록 (GAL)에서 Microsoft 365 그룹을 숨기려면 EXO shell에서 다음 명령을 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="4fe4b-103">To hide a Microsoft 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="4fe4b-104">Microsoft 365 그룹을 Exchange 클라이언트에 표시 하지 않도록 숨기려면 EXO shell에서 다음 명령을 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="4fe4b-104">To hide the Microsoft 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

