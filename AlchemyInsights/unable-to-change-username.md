---
title: 사용자 이름을 변경할 수 없음
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 3088a7b939e7b88319ff688ea94fa71d7fa540787cde31cfd864551113caf149
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020234"
---
# <a name="unable-to-change-username"></a>사용자 이름을 변경할 수 없음

경우에 따라 UPN(UserPrincipalName) 변경 내용이 클라우드에 전파되지 않습니다. Office 365 포털에서 유효성 검사 오류를 수신하거나 사용자 이름 또는 전자 메일 주소를 변경하지 못할 수 있습니다. 이 문제를 해결 하려면 이 PowerShell 명령을 사용하여 수동으로 UserPrincipalName을 설정합니다.

**예: 사용자 이름 바꾸기**

PowerShellCopy

PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

이 명령으로 davidc@contoso.com에서 davidchew@contoso.com으로 이름이 변경됩니다.

자세한 내용은 [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0)을 참조하세요.