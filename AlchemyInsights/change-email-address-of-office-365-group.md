---
title: Microsoft 365 그룹의 전자 메일 주소 변경
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
- "1200024"
- "4704"
ms.openlocfilehash: 6bd9301b983d09f6a0058fee17577b9fc695458ed205f96aacf79a87e4a91e34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930735"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Microsoft 365 그룹의 전자 메일 주소 변경

관리 센터를 사용하여 Microsoft 365 그룹의 전자 메일 주소를 변경할 수 있습니다. 그룹을 선택하고 @전자 메일 주소 편집을 선택하면 됩니다.

다음 EXO PowerShell 명령을 사용하여 Microsoft 365 그룹의 기본 SMTP 주소를 변경할 수도 있습니다.

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

예제:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
