---
title: 팀의 파일 액세스
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
- "2675"
- "9000710"
ms.openlocfilehash: a00a39954737287b4888b833b66d98e9b5e711b2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668533"
---
# <a name="accessing-files-in-microsoft-teams"></a><span data-ttu-id="72827-102">Microsoft 팀의 파일 액세스</span><span class="sxs-lookup"><span data-stu-id="72827-102">Accessing files in Microsoft Teams</span></span>

<span data-ttu-id="72827-103">Microsoft 팀의 파일에 액세스 하기 어려운 경우 먼저 파일이 개인 채팅에 첨부 되었는지 아니면 채널 대화에 연결 되어 있는지를 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="72827-103">If users have difficulty accessing a file in Microsoft Teams, first determine whether the file is attached to a private chat or a channel conversation.</span></span> <span data-ttu-id="72827-104">팀 채널은 팀의 모든 구성원이 개방적으로 대화를 할 수 있는 위치입니다.</span><span class="sxs-lookup"><span data-stu-id="72827-104">Team channels are places where everyone on the team can openly have conversations.</span></span> <span data-ttu-id="72827-105">개인 채팅은 채팅에서 사용자만 볼 수 있고 채팅에서 공유한 파일은 비즈니스용 OneDrive에 저장 됩니다.</span><span class="sxs-lookup"><span data-stu-id="72827-105">Private chats are only visible to those people in the chat (and files that you share in a chat are stored in OneDrive for Business).</span></span>

<span data-ttu-id="72827-106">사용자가 개인 채팅에서 파일을 공유 하는 경우 해당 파일은 공유 사용자의 비즈니스용 OneDrive에 저장 됩니다.</span><span class="sxs-lookup"><span data-stu-id="72827-106">When users share files in private chats, the file is stored on the sharing user's OneDrive for Business.</span></span> <span data-ttu-id="72827-107">기존 개인 채팅에 사용자를 추가 하는 경우 원래 소유자가 파일을 다시 공유 하지 않으면 파일에 액세스할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="72827-107">If a user was added to an existing private chat, they won't be able to access the files unless the original owner re-shares the file.</span></span>    

<span data-ttu-id="72827-108">**채널 대화의 경우:**</span><span class="sxs-lookup"><span data-stu-id="72827-108">**For channel conversations:**</span></span>

- <span data-ttu-id="72827-109">[Microsoft 팀에서 파일을 공유](https://docs.microsoft.com/MicrosoftTeams/sharing-files-in-teams) 하는 기능은 SharePoint 또는 OneDrive에 구성 된 설정을 기반으로 합니다.</span><span class="sxs-lookup"><span data-stu-id="72827-109">[Sharing files in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/sharing-files-in-teams) is based on the settings configured in SharePoint or OneDrive.</span></span> 
- <span data-ttu-id="72827-110">[팀과 파일 공동 작업](https://support.office.com/article/Collaborate-on-files-with-your-Team-9b200289-dbac-4823-85bd-628a5c7bb0ae) 을 검토 하 여 팀이 조직에서 파일을 공유 하 고 공동으로 작업 하는 방법에 대해 자세히 알아볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="72827-110">Review [Collaborate on files with your Team](https://support.office.com/article/Collaborate-on-files-with-your-Team-9b200289-dbac-4823-85bd-628a5c7bb0ae) to learn more about how Teams allows your organization to share and collaborate on files.</span></span> 
- <span data-ttu-id="72827-111">새 팀 구성원이 파일에 액세스 하는 데 지연이 발생 하는 경우에는 **4 시간** 이상 기다린 후에 지원 티켓을 열어 복제가 완료 될 수 있도록 하십시오.</span><span class="sxs-lookup"><span data-stu-id="72827-111">If new team members experience a delay in accessing files, please wait at least **4 hours** before opening a support ticket to allow replication to complete.</span></span> 

<span data-ttu-id="72827-112">사용자가 이전에 팀 채널의 파일 탭을 통해 파일에 액세스할 수 있고 "이러한 파일을 더 이상 사용할 수 없습니다." 라는 오류가 표시 되 면 SharePoint 사이트 또는 문서 라이브러리의 이름이 바뀌었는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="72827-112">If users could previously access files via the Files tab on a team channel, and you get a "these files are no longer available" error, check to see if the SharePoint site or document library has been renamed.</span></span> <span data-ttu-id="72827-113">팀의 SharePoint 사이트 및 문서 라이브러리 이름은 아직 지원 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="72827-113">Renaming SharePoint sites and document libraries for Teams is not yet supported.</span></span> <span data-ttu-id="72827-114">이 문제를 해결 하려면이 팀에 사용 된 팀 사이트를 열고 라이브러리의 이름을 다시 "공유 문서"로 변경 합니다.</span><span class="sxs-lookup"><span data-stu-id="72827-114">To resolve this issue, open the team site used for this team and rename the library back to “Shared Documents”.</span></span>