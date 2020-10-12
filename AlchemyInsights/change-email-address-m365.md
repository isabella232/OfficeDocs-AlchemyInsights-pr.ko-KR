---
title: Microsoft 365 그룹의 전자 메일 주소 변경
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
- "1200024"
- "4704"
ms.openlocfilehash: f54ca5df09d0604f6d58c6c8a41dc907485e1f04
ms.sourcegitcommit: beb9715ac0c8e8333fef6764ecd346b7401a2612
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48416697"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Microsoft 365 그룹의 전자 메일 주소 변경

관리 센터를 사용하여 Microsoft 365 그룹의 전자 메일 주소를 변경할 수 있습니다. 그룹을 선택하고 @전자 메일 주소 편집을 선택하면 됩니다.

다음 EXO PowerShell 명령을 사용하여 Microsoft 365 그룹의 기본 SMTP 주소를 변경할 수도 있습니다.

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

예제:

`et-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
