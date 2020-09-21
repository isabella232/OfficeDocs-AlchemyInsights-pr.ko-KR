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
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Office 365 그룹 또는 팀을 주소 목록에서 숨기기 또는 숨기기 취소

다음 EXO PowerShell 명령을 사용하여 Exchange 클라이언트(Outlook, OWA)의 주소 목록(GAL)에서 Office 365 그룹/팀을 숨기거나 숨기기 취소할 수 있습니다.

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

다음 EXO PowerShell 명령을 사용하여 Exchange 클라이언트(Outlook, OWA)에서 Office 365 그룹/팀을 숨기거나 숨기기 취소할 수 있습니다.

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- 자세한 지침은 [GAL 및 Exchange 클라이언트에서 Office 365 그룹 숨기기](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)를 참조하세요.
