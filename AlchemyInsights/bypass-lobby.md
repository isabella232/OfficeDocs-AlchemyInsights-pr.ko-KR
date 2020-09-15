---
title: 바이패스 로비
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684956"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="25a3a-102">팀에서의 로비 설정 및 참여 수준 제어</span><span class="sxs-lookup"><span data-stu-id="25a3a-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="25a3a-103">전화 접속, 외부 및 익명 사용자를 포함 하 여 모든 사용자가 **로비를 우회**하도록 허용 하려면 PowerShell을 사용 하 여이 작업을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="25a3a-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="25a3a-104">다음은 조직에 대 한 전역 모임 정책을 수정 하는 예입니다.</span><span class="sxs-lookup"><span data-stu-id="25a3a-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="25a3a-105">이 cmdlet은 현재 비즈니스용 Skype PowerShell 모듈을 사용 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="25a3a-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="25a3a-106">이 cmdlet을 사용 하도록 설정 하려면 [PowerShell을 통해 정책 관리](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="25a3a-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="25a3a-107">정책을 설정한 후에는 사용자에 게 적용 해야 합니다. 또는 전역 정책을 수정한 경우 사용자에 게 자동으로 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="25a3a-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="25a3a-108">정책이 변경 되는 경우 정책이 적용 되려면 최소 **24** 시간까지 기다려야 합니다.</span><span class="sxs-lookup"><span data-stu-id="25a3a-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="25a3a-109">이를 변경 하기 전에 아래의 설명서를 검토 하 여 해당 작업을 정확히 이해 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="25a3a-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="25a3a-110">팀 모임 로비 정책 컨트롤 이해</span><span class="sxs-lookup"><span data-stu-id="25a3a-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="25a3a-111">이러한 설정은 모임에 참가 하기 전에 로비에서 대기 하는 모임 참가자 및 모임에서 허용 되는 참여 수준을 제어 합니다.</span><span class="sxs-lookup"><span data-stu-id="25a3a-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="25a3a-112">PowerShell을 사용 하 여 팀 관리 센터에서 아직 구현 되지 않은 모임 정책 설정 ("출시 예정")을 업데이트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="25a3a-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="25a3a-113">모든 사용자가 로비를 무시할 수 있도록 하는 예제 PowerShell cmdlet은 아래를 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="25a3a-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="25a3a-114">사용자가 인증 된 사용자가 참석할 수 있을 때까지 사용자가 모임에 직접 참가 하거나 로비에서 대기할지 여부를 제어 하는 이끌이 별 정책 [으로 자동으로 인정](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) 합니다.</span><span class="sxs-lookup"><span data-stu-id="25a3a-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="25a3a-115">[익명 사용자가 모임을 시작할 수 있도록 허용](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) 은 B2B 및 페더레이션 사용자를 비롯 한 익명 사용자가 사용자의 모임에 참석할 수 있는지 여부를 제어 하는 이끌이 별 정책입니다.</span><span class="sxs-lookup"><span data-stu-id="25a3a-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="25a3a-116">전화 [접속 사용자의 로비 사용 허용](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**출시 예정**)은 전화로 전화를 거는 사용자가 모임에 직접 참가할 지 또는 **자동 허용 사용자** 설정에 관계 없이 로비에서 대기할지 여부를 제어 하는 이끌이 별 정책입니다.</span><span class="sxs-lookup"><span data-stu-id="25a3a-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="25a3a-117">[이끌이가 로비 설정 재정의 허용](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**곧 예정**)은 모임 이끌이가 관리자가 **자동으로 사용자** **를 허용 하 고 전화 접속 사용자가** 새 모임을 예약할 때 로비를 우회 하도록 할 수 있는지 여부를 제어 하는 이끌이 별 정책입니다.</span><span class="sxs-lookup"><span data-stu-id="25a3a-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="25a3a-118">**참고:** Microsoft 팀 회의 정책에 대 한 전체 개요를 보려면 [팀에서 모임 정책 관리](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) 를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="25a3a-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
