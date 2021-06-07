---
title: Teams 웨비나 사용
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760856"
---
# <a name="enable-teams-webinars"></a><span data-ttu-id="6ebad-102">Teams 웨비나 사용</span><span class="sxs-lookup"><span data-stu-id="6ebad-102">Enable Teams Webinars</span></span>

<span data-ttu-id="6ebad-103">웨비나는 기본적으로 사용하도록 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="6ebad-103">Webinars are enabled by default.</span></span> <span data-ttu-id="6ebad-104">Teams PowerShell 명령을 사용하여 Teams 웨비나를 예약하고 등록할 수 있는 사용자를 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6ebad-104">You can manage who can schedule and register for Teams Webinars by using Teams PowerShell commands.</span></span>

- <span data-ttu-id="6ebad-105">모임을 만들 수 있는 모든 사용자는 웨비나 모임도 만들 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6ebad-105">All users who can create a meeting can also create a webinar meeting.</span></span> <span data-ttu-id="6ebad-106">Teams 웨비나를 예약할 수 있는 사용자를 관리하려면 *AllowMeetingRegistration* 을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="6ebad-106">If you want to manage who can schedule Teams Webinars, use *AllowMeetingRegistration*.</span></span> 
- <span data-ttu-id="6ebad-107">기본적으로 *WhoCanRegister* 사용하도록 설정되고 **Everyone** 로 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="6ebad-107">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="6ebad-108">모임 등록을 끄려면 *AllowMeetingRegistration* 을 **False** 로 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="6ebad-108">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="6ebad-109">이러한 설정을 변경하려면 [Teams PowerShell](/microsoftteams/teams-powershell-install)을 설치해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="6ebad-109">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="6ebad-110">또한 모임 정책이 Teams 웨비나에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="6ebad-110">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="6ebad-111">예를 들어 모임 설정에서 익명 참가가 해제된 경우 익명 사용자는 웨비나에 참가할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="6ebad-111">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="6ebad-112">웨비나에 등록할 수 있는 사용자를 구성하는 방법에 대한 자세한 내용은 [웨비나에 등록할 수 있는 사용자 구성](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="6ebad-112">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="6ebad-113">Microsoft Lists의 설정에 대한 자세한 내용은 [Microsoft Lists에 대한 컨트롤 설정](/sharepoint/control-lists)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="6ebad-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>