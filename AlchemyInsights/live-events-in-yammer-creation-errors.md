---
title: Yammer 라이브 이벤트 만들기 오류
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
- "9002495"
- "5112"
ms.openlocfilehash: 383943d670c935403fb7f4466a72474120e27e7a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825521"
---
# <a name="live-events-in-yammer-creation-errors"></a><span data-ttu-id="af224-102">Yammer 라이브 이벤트 만들기 오류</span><span class="sxs-lookup"><span data-stu-id="af224-102">Live events in Yammer creation errors</span></span>

<span data-ttu-id="af224-103">**Yammer 라이브 이벤트 만들기**</span><span class="sxs-lookup"><span data-stu-id="af224-103">**Yammer Live Event creation**</span></span>

<span data-ttu-id="af224-104">Yammer에는 항상 라이브 이벤트를 만들 수 있는 옵션이 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="af224-104">Yammer will show the option to create a live event at all times.</span></span> <span data-ttu-id="af224-105">경우에 따라 사용자가 라이브 이벤트를 만들기를 위한 필수 조건을 충족하지 못하여 만들려고 하면 오류가 발생하는 경우도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="af224-105">In some cases, a user may not meet the prerequisites for creating a live event and receive an error when they attempt to create it.</span></span> <span data-ttu-id="af224-106">아래 항목에서는 이 문제의 일반적인 원인을 다루며 최종 사용자에게 이 문제를 해결하는 방법을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="af224-106">The items below cover common reasons for this problem and provide ways to resolve it for end users.</span></span>

<span data-ttu-id="af224-107">**라이브 이벤트를 만들 수 있는 사용자**</span><span class="sxs-lookup"><span data-stu-id="af224-107">**Who can create live events**</span></span>
- <span data-ttu-id="af224-108">Office 365 Enterprise E1, E3 또는 E5 라이선스 또는 Office 365 A3 또는 A5 라이선스.</span><span class="sxs-lookup"><span data-stu-id="af224-108">An Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license.</span></span>
- <span data-ttu-id="af224-109">Microsoft Teams 관리 센터에서 라이브 이벤트를 만들기 위한 권한.</span><span class="sxs-lookup"><span data-stu-id="af224-109">Permission to create live events in Microsoft Teams admin center.</span></span>
- <span data-ttu-id="af224-110">Microsoft Stream에서 라이브 이벤트를 만들기 위한 권한(외부 브로드캐스팅 앱 또는 디바이스를 사용하여 생성한 이벤트용).</span><span class="sxs-lookup"><span data-stu-id="af224-110">Permission to create live events in Microsoft Stream (for events produced using an external broadcasting app or device).</span></span>
- <span data-ttu-id="af224-111">조직의 전체 팀 구성원 자격(게스트 또는 다른 조직의 구성원 자격은 제외).</span><span class="sxs-lookup"><span data-stu-id="af224-111">Full team membership in the org (can’t be a guest or from another org).</span></span>
- <span data-ttu-id="af224-112">팀 모임 정책에 설정된 비공개 모임 예약, 화면 공유 및 IP 비디오 공유.</span><span class="sxs-lookup"><span data-stu-id="af224-112">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

<span data-ttu-id="af224-113">**라이브 이벤트 만들기 정책**</span><span class="sxs-lookup"><span data-stu-id="af224-113">**Live event creation policies**</span></span>

<span data-ttu-id="af224-114">Yammer는 스트림의 Office 365 테넌트에 설정된 라이브 이벤트 정책을 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="af224-114">Yammer follows the Live Event policies set in your Office 365 tenant for Stream.</span></span> <span data-ttu-id="af224-115">기본적으로 조직의 모든 사용자가 라이브 이벤트를 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="af224-115">By default, everyone in your organization can create a live event.</span></span> <span data-ttu-id="af224-116">관리자는 [사용자가 라이브 이벤트를 만들지 못하도록 할 수 있는 이 설정을 변경](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating)할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="af224-116">Administrators may [make changes to this setting which may prevent users from creating a live event](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span></span> <span data-ttu-id="af224-117">사용자에게 정책 오류가 발생하는 경우 라이브 이벤트를 만들 수 있는 권한이 있는지 확인하는 것이 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="af224-117">It is important to check that users have permissions to create live events if they receive a policy error.</span></span>
