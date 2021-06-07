---
title: 웹비나 등록 관리
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783142"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="9ce59-102">웹비나 등록 관리</span><span class="sxs-lookup"><span data-stu-id="9ce59-102">Manage webinar registration</span></span>

<span data-ttu-id="9ce59-103">Teams PowerShell 명령을 사용하여 Teams 웨비나에 등록할 수 있는 사용자를 관리합니다.</span><span class="sxs-lookup"><span data-stu-id="9ce59-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="9ce59-104">Teams Powershell을 설치하려면 [Teams PowerShell](/microsoftteams/teams-powershell-install)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="9ce59-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="9ce59-105">기본적으로 *WhoCanRegister* 는 사용하도록 설정되고 **EveryoneInCompany** 로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="9ce59-105">By default, *WhoCanRegister* is enabled and set to **EveryoneInCompany**.</span></span> <span data-ttu-id="9ce59-106">익명 사용자를 포함한 모든 사용자가 등록할 수 있도록 하려면 Powershell 명령을 사용하여 모임 정책을 **모든 사용자** 로 설정해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="9ce59-106">To allow anyone, including anonymous users, to register, you must set the Meeting Policy to **Everyone** by using the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="9ce59-107">**참고**: 모임 설정에서 익명 참가가 해제된 경우 익명 사용자는 웨비나에 참가할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="9ce59-107">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="9ce59-108">자세한 내용을 알아보고 이 설정을 사용하도록 설정하려면 [Microsoft Teams에서 모임 설정 관리](/microsoftteams/meeting-settings-in-teams)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="9ce59-108">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="9ce59-109">모임 등록을 끄려면 *AllowMeetingRegistration* 을 **False** 로 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="9ce59-109">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="9ce59-110">웨비나에 등록할 수 있는 사용자를 구성하는 방법에 대한 자세한 내용은 [웨비나에 등록할 수 있는 사용자 구성](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="9ce59-110">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="9ce59-111">Microsoft Lists의 설정에 대한 자세한 내용은 [Microsoft Lists에 대한 컨트롤 설정](/sharepoint/control-lists)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="9ce59-111">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
