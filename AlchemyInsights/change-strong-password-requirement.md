---
title: 강력한 암호 요구 사항 변경
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
- "9000105"
- "1600"
ms.openlocfilehash: cf5cab9a1c2dd4226997d93417dc7104347f8a6e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818474"
---
# <a name="change-strong-password-requirement"></a>강력한 암호 요구 사항 변경

Microsoft에는 기본적으로 강력한 암호가 필요합니다.

PowerShell을 사용하여 다음 명령을 사용하여 특정 사용자에 대해 강력한 암호를 사용하지 않도록 설정할 수 있습니다.

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

모든 사용자에 대해 강력한 암호를 사용하지 않도록 설정하기 위해 다음을 사용하세요.

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [암호 정책에 대한 자세한 정보](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [PowerShell을 사용하여 Microsoft 365에 연결하는 방법](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [PowerShell MsolUser 명령에 대한 자세한 정보](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
