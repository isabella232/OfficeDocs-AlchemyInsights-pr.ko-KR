---
title: Microsoft Teams 클라이언트에 일정 아이콘이 표시되지 않습니다.
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576520"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a><span data-ttu-id="76456-102">Microsoft Teams 클라이언트에 일정 아이콘이 표시되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="76456-102">Calendar icon isn't showing in Microsoft Teams client</span></span>

<span data-ttu-id="76456-103">**Teams의** 일정 탭은 Exchange 웹 서비스를 통해 Exchange 사서함에 액세스해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="76456-103">The **Calendar** Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="76456-104">Exchange 사서함은 Online 또는 On-Premises일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="76456-104">The Exchange mailbox can be Online, or On-Premises.</span></span> <span data-ttu-id="76456-105">일정 탭이 없는 온라인 **Calendar** 사용자의 경우 Exchange Online 사서함에 대한 라이선스가 부여되어 있으며 사서함이 사용하도록 [설정되어 있는지 확인합니다.](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes)</span><span class="sxs-lookup"><span data-stu-id="76456-105">For Online users who do not see the **Calendar** Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span> <span data-ttu-id="76456-106">사용자가 홈인 경우 하이브리드 구성이 정상 상태인지 확인해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="76456-106">If your users are homed On-Premises, you need to confirm that your Hybrid configuration is healthy.</span></span> <span data-ttu-id="76456-107">[하이브리드 구성 마법사](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent)를 사용하여 문제를 해결하십시오.</span><span class="sxs-lookup"><span data-stu-id="76456-107">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span> <span data-ttu-id="76456-108">[Teams는 Exchange 2016 CU3 이상을 필요](https://docs.microsoft.com/microsoftteams/exchange-teams-interact)로 합니다.</span><span class="sxs-lookup"><span data-stu-id="76456-108">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>

<span data-ttu-id="76456-109">자세한 정보 및 문제 해결 단계는 Microsoft Teams 문제 해결을 참조하고 상호 [작용 Exchange Server 참조하세요.](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue)</span><span class="sxs-lookup"><span data-stu-id="76456-109">For more information and troubleshooting steps, see [Troubleshoot Microsoft Teams and Exchange Server interaction issues](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span></span>
