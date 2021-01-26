---
title: 보관 사서함이 거의 가득 차 있습니다.
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950510"
---
# <a name="your-archive-mailbox-is-almost-full"></a><span data-ttu-id="d0e01-102">보관 사서함이 거의 가득 차는 경우</span><span class="sxs-lookup"><span data-stu-id="d0e01-102">Your archive mailbox is almost full</span></span>

<span data-ttu-id="d0e01-103">사용자가 경고를 받는 경우 **보관 사서함이 거의 가득 차거나** 보관 사서함의 크기를 늘려야 합니다. 몇 가지 팁은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="d0e01-103">If the user receives the warning; **Your archive mailbox is almost full**, or you need to increase the size of their archive mailbox, here are some tips:</span></span>

1. <span data-ttu-id="d0e01-104">사용자에게 Exchange Online 계획 1이 할당된 경우 크기를 50GB에서 100GB로 늘리기 위해 **Exchange Online 계획 2** 라이선스로 업그레이드합니다.</span><span class="sxs-lookup"><span data-stu-id="d0e01-104">If the user is assigned an Exchange Online Plan 1, upgrade to **Exchange Online Plan 2** license to increase the size from 50 GB to 100GB.</span></span>
1. <span data-ttu-id="d0e01-105">사용자에게 이미 할당된 기능 중 하나인 **Exchange Online 계획 2** 또는 Exchange Online Archiving 추가 기능을 사용하는 Exchange Online 계획 1을 사용하려면 아래 단계를 사용하여 자동 확장 보관을 사용하도록 설정하십시오.</span><span class="sxs-lookup"><span data-stu-id="d0e01-105">If the user is already assigned either of the following: **Exchange Online Plan 2** or an Exchange Online Plan 1 with an Exchange Online Archiving add-on, use the steps below to enable Auto-Expanding archiving:.</span></span>
 
    1. <span data-ttu-id="d0e01-106">[Exchange Online Powershell에 연결합니다.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="d0e01-106">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>
    2. <span data-ttu-id="d0e01-107">사용자에 대해 다음 commandlet을 실행합니다.  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span><span class="sxs-lookup"><span data-stu-id="d0e01-107">Run the following commandlet for the user:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span></span>
    1. <span data-ttu-id="d0e01-108">다음 commandlet을 실행하여 사용자가 사용할 수 있도록 설정되어 있는지 확인합니다.  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span><span class="sxs-lookup"><span data-stu-id="d0e01-108">Run the following commandlet to confirm it is enabled for the user:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span></span>

<span data-ttu-id="d0e01-109">자세한 내용은 다음을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="d0e01-109">For more information see:</span></span>

- [<span data-ttu-id="d0e01-110"> 무제한 보관 사용 - 관리자 도움말 - Microsoft 365 규정 준수 | Microsoft Docs</span><span class="sxs-lookup"><span data-stu-id="d0e01-110"> Enable unlimited archiving - Admin Help - Microsoft 365 Compliance | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [<span data-ttu-id="d0e01-111">Exchange Online 제한 - 서비스 설명 | Microsoft Docs</span><span class="sxs-lookup"><span data-stu-id="d0e01-111">Exchange Online limits - Service Descriptions | Microsoft Docs</span></span>](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [<span data-ttu-id="d0e01-112">다른 비즈니스 계획 계획 | Microsoft Docs</span><span class="sxs-lookup"><span data-stu-id="d0e01-112">Upgrade to a different business plan | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

