---
title: 주소 목록에서 그룹을 숨기거나 숨기기지 않는 지침
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
- "1200024"
- "3161"
ms.openlocfilehash: af7085890d295cf0c41e11aaf18e404313413100cb8a1134bfac051d5fa26996
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926251"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>GAL(Microsoft 365 그룹 숨기기)

Microsoft 365 클라이언트(예: Outlook 또는 OWA)의 Exchange GAL(주소 목록)에서 Outlook 그룹을 숨기기 위해 EXO 셸에서 다음 명령을 사용하세요.

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

클라이언트에서 Microsoft 365 그룹이 표시되지 Exchange 숨기기 위해 EXO 셸에서 다음 명령을 사용 합니다.

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

