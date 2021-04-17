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
# <a name="change-strong-password-requirement"></a><span data-ttu-id="b5324-102">강력한 암호 요구 사항 변경</span><span class="sxs-lookup"><span data-stu-id="b5324-102">Change strong password requirement</span></span>

<span data-ttu-id="b5324-103">Microsoft에는 기본적으로 강력한 암호가 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="b5324-103">Microsoft requires strong passwords by default.</span></span>

<span data-ttu-id="b5324-104">PowerShell을 사용하여 다음 명령을 사용하여 특정 사용자에 대해 강력한 암호를 사용하지 않도록 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b5324-104">Using PowerShell, you can disable strong passwords for specific users with these commands:</span></span>

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

<span data-ttu-id="b5324-105">모든 사용자에 대해 강력한 암호를 사용하지 않도록 설정하기 위해 다음을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="b5324-105">To disable strong passwords for all users, use:</span></span>

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [<span data-ttu-id="b5324-106">암호 정책에 대한 자세한 정보</span><span class="sxs-lookup"><span data-stu-id="b5324-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="b5324-107">PowerShell을 사용하여 Microsoft 365에 연결하는 방법</span><span class="sxs-lookup"><span data-stu-id="b5324-107">How to connect to Microsoft 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="b5324-108">PowerShell MsolUser 명령에 대한 자세한 정보</span><span class="sxs-lookup"><span data-stu-id="b5324-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
