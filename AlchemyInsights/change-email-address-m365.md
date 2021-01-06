---
title: Microsoft 365 그룹 또는 Microsoft Teams의 전자 메일 주소 변경
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
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756563"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Microsoft 365 그룹 또는 Microsoft Teams의 전자 메일 주소 변경

[Microsoft 365 관리 센터](https://admin.microsoft.com/)를 사용하여 Microsoft 365 그룹 또는 Microsoft Teams의 전자 메일 주소를 변경할 수 있습니다. 그룹을 선택하고 @전자 메일 주소 편집을 선택하면 됩니다.

다음 EXO PowerShell 명령을 사용하여 Microsoft 365 그룹/Teams의 기본 SMTP 주소를 변경할 수도 있습니다.

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

예제:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
