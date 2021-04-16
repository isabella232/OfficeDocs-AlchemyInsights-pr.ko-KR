---
title: 정책 catchall
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
- "9000734"
- "3207"
ms.openlocfilehash: 036c171f3c71e60c8c07000b4d0c6ede36bd435c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51801672"
---
# <a name="teams-policies"></a><span data-ttu-id="9dc0b-102">Teams 정책</span><span class="sxs-lookup"><span data-stu-id="9dc0b-102">Teams policies</span></span>

<span data-ttu-id="9dc0b-103">Microsoft Teams 설정은 정책에 의해 제어됩니다.</span><span class="sxs-lookup"><span data-stu-id="9dc0b-103">Microsoft Teams settings are controlled by policies.</span></span> <span data-ttu-id="9dc0b-104">변경하려면 적절한 정책을 구성한 다음 사용자에게 적용해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="9dc0b-104">To make a change, you must configure the appropriate policy, and then apply it to users.</span></span> <span data-ttu-id="9dc0b-105">모든 사용자에 대해 이 작업을 가장 빠르게 하는 방법은 Global이라는 기본 정책을 수정하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="9dc0b-105">The quickest way to do this for all your users is to modify the default policy named Global.</span></span> 

<span data-ttu-id="9dc0b-106">**참고** 정책 변경 내용을 적용하는 데 **_최소 4시간에서 48시간까지 소요됩니다._**</span><span class="sxs-lookup"><span data-stu-id="9dc0b-106">**NOTE** Policy changes take **_at least 4 up to 48 hours to take effect_**.</span></span> <span data-ttu-id="9dc0b-107">사용자 지정 정책을 만드는 경우 4시간 이상 기다렸다가 추가 변경을 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="9dc0b-107">If you create a custom policy, you need to wait at least 4 hours before you can make additional changes to it.</span></span> <span data-ttu-id="9dc0b-108">그런 다음 해당 정책을 사용자에게 적용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9dc0b-108">Then you can apply that policy to users.</span></span> <span data-ttu-id="9dc0b-109">즉, 사용자 지정 정책을 적용하는 데 최대 48시간이 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9dc0b-109">This means that custom policies can take up to 48 hours to take effect.</span></span> <span data-ttu-id="9dc0b-110">전역 정책은 모든 사용자에 대해 기본 정책으로 설정되어 있으며 글로벌 정책에 대한 변경 내용을 적용하는 데 최대 24시간이 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9dc0b-110">Global policies are set as default for all users, and changes to the Global policy can take up to 24 hours to take effect.</span></span> <span data-ttu-id="9dc0b-111">사용자 지정 정책을 만들어 사용자에게 적용한 경우 48시간이 지난 후에도 적용되지 않은 경우 또는 글로벌 정책을 수정하고 24시간 이상 기다렸다면 지원 사례를 열 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9dc0b-111">If you have created a custom policy, applied it to users, and it still hasn't taken effect after 48 hours, or you've modified the Global policy and waited at least 24 hours, please open a support case.</span></span>

<span data-ttu-id="9dc0b-112">Teams 정책은 다음 영역으로 나뉘어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9dc0b-112">Teams policies are divided into the following areas:</span></span>

- <span data-ttu-id="9dc0b-113">[Teams 정책은](https://docs.microsoft.com/MicrosoftTeams/teams-policies) 비공개 채널의 검색 및 생성에서 비공개 팀의 사용자 검색을 제어합니다.</span><span class="sxs-lookup"><span data-stu-id="9dc0b-113">[Teams policies](https://docs.microsoft.com/MicrosoftTeams/teams-policies) control user discovery of private teams in search and creation of private channels.</span></span>  
- <span data-ttu-id="9dc0b-114">[모임 정책은](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) 대기실 제어를 포함하여 Teams 모임에서 사용자가 할 수 있는 작업을 제어합니다.</span><span class="sxs-lookup"><span data-stu-id="9dc0b-114">[Meeting policies](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) control what users can do with Teams meetings, including controlling the lobby.</span></span> <span data-ttu-id="9dc0b-115">모든 사람을 참가할 수 있도록 Teams를 구성하는 등 대기실 문제에 대한 도움말은 대기실 설정 및 참가 수준 [제어를 참조하세요.](https://docs.microsoft.com/alchemyinsights/bypass-lobby)</span><span class="sxs-lookup"><span data-stu-id="9dc0b-115">For help with lobby issues, like configuring Teams to admit everyone, see [Control lobby settings and levels of participation](https://docs.microsoft.com/alchemyinsights/bypass-lobby).</span></span>
- <span data-ttu-id="9dc0b-116">[메시징 정책은](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) 채팅 설정 또는 해제, 채팅 삭제, 읽은 확인 요청, Giphy 및 스티커 사용 등을 포함하여 사용자가 채팅 및 메시지로 할 수 있는 작업을 제어합니다.</span><span class="sxs-lookup"><span data-stu-id="9dc0b-116">[Messaging policies](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) control what users can do with chat and messages, including turning chat on or off, deleting chats, requesting read receipts, using giphys and stickers, and more.</span></span>
- <span data-ttu-id="9dc0b-117">[앱 설정 정책은](https://docs.microsoft.com/MicrosoftTeams/teams-app-setup-policies) 사용자 지정 및 타사 앱을 포함하여 사용자가 사용할 수 있는 앱과 앱이 나타나는 순서를 제어합니다.</span><span class="sxs-lookup"><span data-stu-id="9dc0b-117">[App setup policies](https://docs.microsoft.com/MicrosoftTeams/teams-app-setup-policies) control which apps are available to users, including custom and third-party apps, and the order in which they appear.</span></span>  
- <span data-ttu-id="9dc0b-118">Teams에 [대한](https://docs.microsoft.com/microsoftteams/retention-policies) 데이터 보존 정책은 Microsoft 365 보안 및 준수 센터에서 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9dc0b-118">Data [retention policies](https://docs.microsoft.com/microsoftteams/retention-policies) for Teams are found in the Microsoft 365 security and Compliance Center.</span></span>
- <span data-ttu-id="9dc0b-119">Teams 주소 책 정책은 범위가 지정한 디렉터리 [검색을 통해 설정됩니다.](https://docs.microsoft.com/MicrosoftTeams/teams-scoped-directory-search)</span><span class="sxs-lookup"><span data-stu-id="9dc0b-119">Teams address book policies are set via [scoped directory search](https://docs.microsoft.com/MicrosoftTeams/teams-scoped-directory-search).</span></span>