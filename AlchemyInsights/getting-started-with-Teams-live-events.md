---
title: Teams 라이브 이벤트 시작
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
- "9000208"
- "3436"
ms.openlocfilehash: a10f756fc69a7a135446d8d3bcec1f5e951627d8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811966"
---
# <a name="getting-started-with-teams-live-events"></a><span data-ttu-id="bf051-102">Teams 라이브 이벤트 시작</span><span class="sxs-lookup"><span data-stu-id="bf051-102">Getting started with Teams live events</span></span>

<span data-ttu-id="bf051-103">Microsoft Teams 라이브 이벤트는 대규모 온라인 사용자에게 스트리밍되는 이벤트를 예약하고 생성할 수 있게 해 주는 Team 모임의 확장입니다.</span><span class="sxs-lookup"><span data-stu-id="bf051-103">Microsoft Teams live events are an extension of Teams meetings that enable you to schedule and produce events that stream to large online audiences.</span></span>

<span data-ttu-id="bf051-104">라이브 이벤트를 만들려면 다음이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="bf051-104">To create a live event, you will need the following:</span></span>

- <span data-ttu-id="bf051-105">먼저, Teams 라이브 이벤트가 [사용자의 국가 및 지역에서 사용이 가능](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability)한지를 확인합니다. 라이브 이벤트는 일부 국가에서는 아직 지원되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="bf051-105">First, confirm that Teams Live Events are [available in your Country and Region](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); Live Events are not yet supported in some countries.</span></span>  <span data-ttu-id="bf051-106">라이선스를 할당하고 정책을 설정했지만 여전히 Teams 라이브 이벤트를 만들 수 없는 경우, 라이브 이벤트를 아직 사용할 수 없는 국가나 지역에 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bf051-106">If you’ve assigned licenses and set policies, but still cannot create a Teams Live Event, it is likely you are in a Country or Region where Live Events is not yet available.</span></span>

- <span data-ttu-id="bf051-107">[Office 365 Enterprise E1, E3 또는 E5 라이선스 또는 Office 365 A3 또는 A5 라이선스](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="bf051-107">An [Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span></span> <span data-ttu-id="bf051-108">**참고**: 최근 Teams 사용량이 증가하여 Teams 라이선스를 사용자에게 할당할 경우 완전히 설정할 때까지 24시간 정도 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bf051-108">**Note**: Due to a recent increase in Teams usage, when you assign a Teams license to a user, it may take around 24 hours before they'll be fully set up.</span></span> <span data-ttu-id="bf051-109">그런 다음, Teams 정책을 할당할 수 없으며 전화 및 오디오 회의와 같은 일부 Teams 기능에 액세스하지 못할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bf051-109">Until then, you won't be able to assign Teams policies to them, and they might not have access to some Teams features like calling and audio conferencing.</span></span>

- <span data-ttu-id="bf051-110">[Microsoft Teams 관리 센터에서 라이브 이벤트를 만들기 위한](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy) 권한</span><span class="sxs-lookup"><span data-stu-id="bf051-110">Permission to [create live events in Microsoft Teams admin center](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span></span>

- <span data-ttu-id="bf051-111">[Microsoft Stream에서 라이브 이벤트를 만들기 위한](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) 권한(외부 브로드캐스팅 앱 도는 디바이스를 사용하여 생성한 이벤트용)</span><span class="sxs-lookup"><span data-stu-id="bf051-111">Permission to [create live events in Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (for events produced using an external broadcasting app or device).</span></span>

- <span data-ttu-id="bf051-112">조직의 전체 팀 구성원 자격(게스트 또는 다른 조직의 구성원)</span><span class="sxs-lookup"><span data-stu-id="bf051-112">Full team membership in the org (can't be a guest or from another org).</span></span>
<span data-ttu-id="bf051-113">팀 모임 정책에 프라이빗 모임 예약, 화면 공유, IP 비디오 공유 설정</span><span class="sxs-lookup"><span data-stu-id="bf051-113">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

- <span data-ttu-id="bf051-114">Teams 라이브 이벤트에 대한 [모범 사례](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42)</span><span class="sxs-lookup"><span data-stu-id="bf051-114">[Best practices](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) for Teams Live Events.</span></span>

<span data-ttu-id="bf051-115">자세한 내용은 [Microsoft Teams 라이브 이벤트 시작](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="bf051-115">For more information, please see [Get started with Microsoft Teams live events](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span></span>