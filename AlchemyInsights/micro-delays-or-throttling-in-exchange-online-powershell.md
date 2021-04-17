---
title: Exchange Online PowerShell의 마이크로 지연 또는 제한
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
- "3500011"
- "5106"
ms.openlocfilehash: 680df9e6e2404ff6b60b17d6ac88e202e9a7bb25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830039"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="73e0e-102">Exchange Online PowerShell의 마이크로 지연 또는 제한</span><span class="sxs-lookup"><span data-stu-id="73e0e-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="73e0e-103">Exchange Online에서 스크립트와 cmdlet을 실행할 때 "마이크로 지연이 적용 됨"이라는 경고 혹은 지연이 표시될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="73e0e-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="73e0e-104">이와 관련된 두 가지 제안 사항은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="73e0e-104">Here are two suggestions related to this:</span></span>

- <span data-ttu-id="73e0e-105">REST API를 기반으로 하며 성능이 크게 향상된 CMDlets을 포함하는 [Exchange Online v2 PowerShell 모듈](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps)을 사용해 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="73e0e-105">You might want to try using the [Exchange Online v2 PowerShell module](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="73e0e-106">이는 자주 사용하는 많은 Get-Cmdlet에는 훌륭한 솔루션이 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="73e0e-106">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="73e0e-107">아직 V2 모듈에서 다루지 않는 Cmdlet을 사용해야 하는 경우, Exchange Online에서 예상되는 PowerShell 제한 사항을 해결하는 방법에 대해 다루는 [Office 365에서 사용자 수가 많은 경우 PowerShell cmdlet을 실행](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="73e0e-107">If you need to use CMDlets that are not covered in the v2 module yet, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around expected PowerShell throttling limits in Exchange Online.</span></span>
