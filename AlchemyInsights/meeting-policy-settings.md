---
title: 모임 정책 설정
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
- "9000734"
- "2657"
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704612"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="42c5d-102">Microsoft Teams에서 모임 정책 관리</span><span class="sxs-lookup"><span data-stu-id="42c5d-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="42c5d-103">**참고: 정책 변경 내용이 사용자에게 적용될 경우 최대 24시간이 걸릴 수 있습니다.**</span><span class="sxs-lookup"><span data-stu-id="42c5d-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="42c5d-104">새로 만든 정책을 즉시 변경하지 못하게 될 수 있습니다. 4시간을 기다렸다가 새로 만든 정책을 다시 수정하려고 합니다.</span><span class="sxs-lookup"><span data-stu-id="42c5d-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="42c5d-105">모임 정책은 조직의 사용자가 예약한 모임에 대해 모임 참가자가 사용할 수 있는 기능을 제어하는 데 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="42c5d-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="42c5d-106">모임 정책의 일부 기능은 아직 Teams 관리 센터에서 구현되지 않을 수 있습니다(설명서에서 "곧 제공될 예정"으로 레이블이 지정되어 있습니다).</span><span class="sxs-lookup"><span data-stu-id="42c5d-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="42c5d-107">이 경우 또는 Microsoft Teams 관리 센터에서 "지금 정책을 업데이트할 수 없지만 나중에 다시 시도하십시오."라는 오류가 발생하는 경우 PowerShell을 사용하여 Teams 모임 정책을 만들거나 수정하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="42c5d-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="42c5d-108">모임 정책에 대한 자세한 내용은 다음 리소스를 참조하십시오.</span><span class="sxs-lookup"><span data-stu-id="42c5d-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="42c5d-109">정책을 만들고, 변경하고, 사용자를 정책에 할당하는 방법을 알아보는 자세한 내용은 Teams에서 모임 정책 [관리를 참조합니다.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="42c5d-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="42c5d-110">PowerShell cmdlet을 사용하여 정책을 변경하기 위해 [Teams PowerShell 개요를 참조하세요.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="42c5d-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="42c5d-111">Teams 모임 정책에 [비즈니스용 Skype PowerShell](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) 모듈을 사용해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="42c5d-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="42c5d-112">자세한 내용은 [\*-CsTeamsMeetingPolicy cmdlet 설명서를](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) 검토하세요.</span><span class="sxs-lookup"><span data-stu-id="42c5d-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

