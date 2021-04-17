---
title: 대기실 우회
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
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820040"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="a4697-102">대기실 설정 및 Teams 참여 수준 제어</span><span class="sxs-lookup"><span data-stu-id="a4697-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="a4697-103">전화 접속, 외부 및 익명 사용자를 비롯한 모든 사용자가 대기실을 우회하도록 허용할 경우 PowerShell을 사용하여 이 작업을 수행할 수 있습니다. </span><span class="sxs-lookup"><span data-stu-id="a4697-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="a4697-104">다음은 조직의 전역 모임 정책을 수정하는 예입니다.</span><span class="sxs-lookup"><span data-stu-id="a4697-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="a4697-105">이 cmdlet은 현재 비즈니스용 Skype PowerShell 모듈을 사용해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a4697-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="a4697-106">이 cmdlet을 사용하기 위한 설정은 [PowerShell을](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)통해 정책 관리를 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="a4697-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="a4697-107">정책을 설정한 후 사용자에게 적용해야 합니다. 또는 글로벌 정책을 수정한 경우 자동으로 사용자에게 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="a4697-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="a4697-108">정책이 변경될 경우 정책이 적용될 때까지 **최소 4시간에서 최대 24시간을** 기다려야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a4697-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="a4697-109">이러한 변경을 통해 허용하는 내용을 정확하게 이해하기 전에 아래 설명서를 검토해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a4697-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="a4697-110">Teams 모임 대기실 정책 컨트롤 이해</span><span class="sxs-lookup"><span data-stu-id="a4697-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="a4697-111">이러한 설정은 모임에 참가하기 전에 대기실에서 대기하는 모임 참가자와 모임에 참가할 수 있는 참가 수준을 제어합니다.</span><span class="sxs-lookup"><span data-stu-id="a4697-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="a4697-112">PowerShell을 사용하여 Teams 관리 센터에서 아직 구현되지 않은 모임 정책 설정("출시 예정"으로 표시)을 업데이트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a4697-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="a4697-113">모든 사용자가 대기실을 우회할 수 있도록 하는 예제 PowerShell cmdlet은 아래를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="a4697-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="a4697-114">[자동으로 사용자](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) 입력은 사용자가 직접 모임에 참가할지 또는 인증된 사용자가 참가할 때까지 대기실에서 대기할지 여부를 제어하는 이끌이 정책입니다.</span><span class="sxs-lookup"><span data-stu-id="a4697-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="a4697-115">[익명 사용자가](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) 모임을 시작할 수 있도록 허용은 B2B 및 페더니트 사용자를 비롯한 익명 사용자가 조직의 인증된 사용자가 참석하지 않고 사용자의 모임에 참가할 수 있는지 여부를 제어하는 이끌이 정책입니다.</span><span class="sxs-lookup"><span data-stu-id="a4697-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="a4697-116">[전화 접속](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) 사용자가 대기실을 우회하도록 허용(곧 출시 예정)은 전화 접속한 사용자가 자동으로 사용자 허용 설정에 관계없이 전화로 모임에 직접 참가할지 또는 대기실에서 대기하는지 여부를 제어하는 이끌이 **정책입니다.** </span><span class="sxs-lookup"><span data-stu-id="a4697-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="a4697-117">[이끌이가](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) 대기실 설정을 무시하도록 허용(출시 예정)은 모임 이끌이가 자동으로 사용자 허용 및 전화 접속 사용자가  새 모임을  예약할 때 대기실을 무시하도록 허용에서 설정한 대기실 설정을 무시할 수 있는지 여부를 제어하는 이끌이 정책입니다.</span><span class="sxs-lookup"><span data-stu-id="a4697-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="a4697-118">**참고:** Microsoft [Teams 모임 정책에](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) 대한 전체 개요는 Teams에서 모임 정책 관리를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="a4697-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
