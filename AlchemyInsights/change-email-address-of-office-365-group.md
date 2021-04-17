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
ms.openlocfilehash: 8eaafae8650a8072cdfbec281afe6d5e93fea655
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819050"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="f2e51-102">Microsoft 365 그룹의 전자 메일 주소 변경</span><span class="sxs-lookup"><span data-stu-id="f2e51-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="f2e51-103">관리 센터를 사용하여 Microsoft 365 그룹의 전자 메일 주소를 변경할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f2e51-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="f2e51-104">그룹을 선택하고 @전자 메일 주소 편집을 선택하면 됩니다.</span><span class="sxs-lookup"><span data-stu-id="f2e51-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="f2e51-105">다음 EXO PowerShell 명령을 사용하여 Microsoft 365 그룹의 기본 SMTP 주소를 변경할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f2e51-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="f2e51-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="f2e51-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="f2e51-107">예제:</span><span class="sxs-lookup"><span data-stu-id="f2e51-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
