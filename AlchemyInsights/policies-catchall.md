---
title: 정책 catchall
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
- "3207"
ms.openlocfilehash: e5d08462e8662fa1651ad81235d0efd5fc4bac58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721300"
---
# <a name="teams-policies"></a><span data-ttu-id="a38b8-102">팀 정책</span><span class="sxs-lookup"><span data-stu-id="a38b8-102">Teams policies</span></span>

<span data-ttu-id="a38b8-103">Microsoft 팀 설정은 정책에 따라 제어 됩니다.</span><span class="sxs-lookup"><span data-stu-id="a38b8-103">Microsoft Teams settings are controlled by policies.</span></span> <span data-ttu-id="a38b8-104">변경을 수행 하려면 적절 한 정책을 구성한 다음 사용자에 게 적용 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a38b8-104">To make a change, you must configure the appropriate policy, and then apply it to users.</span></span> <span data-ttu-id="a38b8-105">모든 사용자에 대해이 작업을 수행 하는 가장 빠른 방법은 Global 이라는 기본 정책을 수정 하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="a38b8-105">The quickest way to do this for all your users is to modify the default policy named Global.</span></span> 

<span data-ttu-id="a38b8-106">**참고 사항** 정책 변경에는 ***최소 4 ~ 48의***시간이 소요 됩니다.</span><span class="sxs-lookup"><span data-stu-id="a38b8-106">**NOTE** Policy changes take ***at least 4 up to 48 hours to take effect***.</span></span> <span data-ttu-id="a38b8-107">사용자 지정 정책을 만드는 경우에는 4 시간 이상 기다린 후에 추가 변경 작업을 수행 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a38b8-107">If you create a custom policy, you need to wait at least 4 hours before you can make additional changes to it.</span></span> <span data-ttu-id="a38b8-108">그런 다음 해당 정책을 사용자에 게 적용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a38b8-108">Then you can apply that policy to users.</span></span> <span data-ttu-id="a38b8-109">즉, 사용자 지정 정책을 적용 하는 데 최대 48 시간이 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a38b8-109">This means that custom policies can take up to 48 hours to take effect.</span></span> <span data-ttu-id="a38b8-110">전역 정책은 모든 사용자에 대해 기본값으로 설정 되 고, 글로벌 정책에 대 한 변경 내용이 적용 되기까지 최대 24 시간이 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a38b8-110">Global policies are set as default for all users, and changes to the Global policy can take up to 24 hours to take effect.</span></span> <span data-ttu-id="a38b8-111">사용자 지정 정책을 만들고 사용자에 게 적용 했지만, 48 시간이 지난 후에도 적용 되지 않았거나, 글로벌 정책을 수정 하 고 24 시간 이상 기다린 경우에는 지원 사례를 여세요.</span><span class="sxs-lookup"><span data-stu-id="a38b8-111">If you have created a custom policy, applied it to users, and it still hasn't taken effect after 48 hours, or you've modified the Global policy and waited at least 24 hours, please open a support case.</span></span>

<span data-ttu-id="a38b8-112">팀 정책은 다음 영역으로 구분 됩니다.</span><span class="sxs-lookup"><span data-stu-id="a38b8-112">Teams policies are divided into the following areas:</span></span>

- <span data-ttu-id="a38b8-113">[팀 정책은](https://docs.microsoft.com/MicrosoftTeams/teams-policies) 개인 채널을 만들고 검색 하는 동안 개인 팀의 사용자 검색을 제어 합니다.</span><span class="sxs-lookup"><span data-stu-id="a38b8-113">[Teams policies](https://docs.microsoft.com/MicrosoftTeams/teams-policies) control user discovery of private teams in search and creation of private channels.</span></span>  
- <span data-ttu-id="a38b8-114">[모임 정책은](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) 로비 제어를 포함 하 여 사용자가 팀 회의를 통해 수행할 수 있는 작업을 제어 합니다.</span><span class="sxs-lookup"><span data-stu-id="a38b8-114">[Meeting policies](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) control what users can do with Teams meetings, including controlling the lobby.</span></span> <span data-ttu-id="a38b8-115">모든 사람을 허용 하도록 팀을 구성 하는 것과 같은 로비 문제에 대 한 도움말은 [제어 로비 설정 및 참여 수준](https://docs.microsoft.com/alchemyinsights/bypass-lobby)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="a38b8-115">For help with lobby issues, like configuring Teams to admit everyone, see [Control lobby settings and levels of participation](https://docs.microsoft.com/alchemyinsights/bypass-lobby).</span></span>
- <span data-ttu-id="a38b8-116">[메시징 정책은](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) 채팅을 설정 하거나 해제 하 고 채팅을 삭제 하 고, 읽음 확인을 요청 하 고, giphys 및 스티커를 사용 하 여 사용자가 채팅 및 메시지를 통해 수행할 수 있는 작업을 제어 합니다.</span><span class="sxs-lookup"><span data-stu-id="a38b8-116">[Messaging policies](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) control what users can do with chat and messages, including turning chat on or off, deleting chats, requesting read receipts, using giphys and stickers, and more.</span></span>
- <span data-ttu-id="a38b8-117">[앱 설치 정책은](https://docs.microsoft.com/MicrosoftTeams/teams-app-setup-policies) 사용자가 사용자 지정 및 타사 앱을 비롯 하 여 어떤 앱을 사용할 수 있는지 제어 하는 데 사용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="a38b8-117">[App setup policies](https://docs.microsoft.com/MicrosoftTeams/teams-app-setup-policies) control which apps are available to users, including custom and third-party apps, and the order in which they appear.</span></span>  
- <span data-ttu-id="a38b8-118">팀에 대 한 데이터 [보존 정책은](https://docs.microsoft.com/microsoftteams/retention-policies) Microsoft 365 보안 및 준수 센터에서 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a38b8-118">Data [retention policies](https://docs.microsoft.com/microsoftteams/retention-policies) for Teams are found in the Microsoft 365 security and Compliance Center.</span></span>
- <span data-ttu-id="a38b8-119">팀 주소록 정책은 [범위 지정 디렉터리 검색](https://docs.microsoft.com/MicrosoftTeams/teams-scoped-directory-search)을 통해 설정 됩니다.</span><span class="sxs-lookup"><span data-stu-id="a38b8-119">Teams address book policies are set via [scoped directory search](https://docs.microsoft.com/MicrosoftTeams/teams-scoped-directory-search).</span></span>