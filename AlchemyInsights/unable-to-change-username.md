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
ms.openlocfilehash: 76891b3abe156b736c3bb6da0f6cd1135346dbe2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798670"
---
# <a name="unable-to-change-username"></a><span data-ttu-id="a3bdb-102">사용자 이름을 변경할 수 없음</span><span class="sxs-lookup"><span data-stu-id="a3bdb-102">Unable to change UserName</span></span>

<span data-ttu-id="a3bdb-103">경우에 따라 UPN(UserPrincipalName) 변경 내용이 클라우드에 전파되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="a3bdb-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="a3bdb-104">Office 365 포털에서 유효성 검사 오류를 수신하거나 사용자 이름 또는 전자 메일 주소를 변경하지 못할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a3bdb-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="a3bdb-105">이 문제를 해결 하려면 이 PowerShell 명령을 사용하여 수동으로 UserPrincipalName을 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="a3bdb-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="a3bdb-106">**예: 사용자 이름 바꾸기**</span><span class="sxs-lookup"><span data-stu-id="a3bdb-106">**Example: Rename a user**</span></span>

<span data-ttu-id="a3bdb-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="a3bdb-107">PowerShellCopy</span></span>

<span data-ttu-id="a3bdb-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="a3bdb-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="a3bdb-109">이 명령으로 davidc@contoso.com에서 davidchew@contoso.com으로 이름이 변경됩니다.</span><span class="sxs-lookup"><span data-stu-id="a3bdb-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="a3bdb-110">자세한 내용은 [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="a3bdb-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>