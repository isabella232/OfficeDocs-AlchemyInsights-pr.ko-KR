---
title: Teams 업그레이드 연기
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
- "2737"
- "4000006"
ms.openlocfilehash: abbf696b1554743bda188704272bfd85fe6f94e2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51801237"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a><span data-ttu-id="f2961-102">Microsoft 주도 Teams 업그레이드를 연기하는 방법</span><span class="sxs-lookup"><span data-stu-id="f2961-102">How to postpone the Microsoft-driven Teams upgrade</span></span>

<span data-ttu-id="f2961-103">**중요:** 지원 진단을 사용하여 이 문제를 해결할 수 있지만 새 관리 센터를 사용하지 않는 것 같습니다.</span><span class="sxs-lookup"><span data-stu-id="f2961-103">**Important**: We can help fix this for you using a support diagnostic, but it looks like you are not using the New Admin Center.</span></span> <span data-ttu-id="f2961-104">새 관리 센터를 사용하려면 오른쪽 위에 새 관리  센터가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="f2961-104">To use the New Admin Center, slide the toggle in the top right that says **new admin center** to the right.</span></span> <span data-ttu-id="f2961-105">새 관리 센터를 사용하여 도움이 **필요하세요?** 위젯을 클릭하고 "Teams 업그레이드 연기"를 입력한 다음 프롬프트에 따라 진단을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="f2961-105">Using the New Admin Center, click the **Need Help?** widget, type "Postpone Teams Upgrade", then follow the prompts to run the diagnostic.</span></span>

<span data-ttu-id="f2961-106">비즈니스용 Skype에서 Microsoft Teams로의 Microsoft 주도 자동 업그레이드에 대한 통신을 받았고 자동화된 업그레이드를 나중에 연기하려면 전역 관리자가 [Teams](https://admin.teams.microsoft.com/dashboard) 관리 포털에 로그인하고 Microsoft Teams 업그레이드에서 상태  새로 고침 단추를 선택한 후 연기 단추를 선택합니다. </span><span class="sxs-lookup"><span data-stu-id="f2961-106">If you received communication about a Microsoft-driven automated upgrade from Skype for Business to Microsoft Teams, and you wish to postpone the automated upgrade to a later date, your Global Admin can log in to the [Teams Admin portal](https://admin.teams.microsoft.com/dashboard) and, after selecting the **Refresh Status** button under Microsoft Teams Upgrade, select the **Postpone** button.</span></span> <span data-ttu-id="f2961-107">테넌트가 Microsoft Teams로 자동 업그레이드하는 새 날짜를 확인하려면 Teams 관리 포털 페이지를 새로 고치십시오.</span><span class="sxs-lookup"><span data-stu-id="f2961-107">To see the new date for your tenant's automated upgrade to Microsoft Teams, refresh the Teams Admin portal page.</span></span>

<span data-ttu-id="f2961-108">**참고:** 연기 **단추는** 자동화된 업그레이드와 관련하여 메시지 센터 알림을 받은 경우만 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f2961-108">**Note:** The **Postpone** button will only be available if you have received the message center notification regarding the automated upgrade.</span></span> 

<span data-ttu-id="f2961-109">전역 관리자는 [Get-CsTeamsUpgradeStatus를](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) 실행하여 현재 업그레이드 상태에 대해 자세히 확인할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f2961-109">Global Admins can also run [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) to learn more about their current upgrade status.</span></span>
