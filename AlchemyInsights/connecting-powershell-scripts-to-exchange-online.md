---
title: PowerShell 스크립트를 Exchange Online에 연결
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6069"
- "3500011"
ms.openlocfilehash: 3a8383a57bc1267311daf03c78841070cca8fb8f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748070"
---
# <a name="connecting-powershell-scripts-to-exchange-online"></a><span data-ttu-id="1fac9-102">PowerShell 스크립트를 Exchange Online에 연결</span><span class="sxs-lookup"><span data-stu-id="1fac9-102">Connecting PowerShell scripts to Exchange Online</span></span>

<span data-ttu-id="1fac9-103">Exchange Online의 기본 인증은 더 이상 사용되지 않으며, 향후 방법은 스크립트와 무인 작업에 인증서 기반 인증을 사용하여 연결하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="1fac9-103">Basic Authentication in Exchange Online is going to be deprecated, and the way forward is to connect by using certificate-based authentication for scripts and unattended tasks.</span></span> <span data-ttu-id="1fac9-104">자세한 내용은 [EXO V2 모듈에서 무인 스크립트를 위한 앱 전용 인증](https://docs.microsoft.com/powershell/exchange/app-only-auth-powershell-v2)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1fac9-104">To learn more, see [App-only authentication for unattended scripts in the EXO V2 module](https://docs.microsoft.com/powershell/exchange/app-only-auth-powershell-v2).</span></span>