---
title: Teams에서 파일에 액세스
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
- "2675"
- "9000710"
ms.openlocfilehash: c6766c318f0058e66950dbd0ca2953b149579a5c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823361"
---
# <a name="accessing-files-in-microsoft-teams"></a><span data-ttu-id="dbaa2-102">Microsoft Teams에서 파일 액세스</span><span class="sxs-lookup"><span data-stu-id="dbaa2-102">Accessing files in Microsoft Teams</span></span>

<span data-ttu-id="dbaa2-103">사용자가 Microsoft Teams에서 파일에 액세스하는 데 어려움이 있는 경우 먼저 파일이 비공개 채팅에 첨부되어 있는지 또는 채널 대화에 첨부되어 있는지를 판단합니다.</span><span class="sxs-lookup"><span data-stu-id="dbaa2-103">If users have difficulty accessing a file in Microsoft Teams, first determine whether the file is attached to a private chat or a channel conversation.</span></span> <span data-ttu-id="dbaa2-104">팀 채널은 팀의 모든 구성원이 개방적으로 대화를 할 수 있는 위치입니다.</span><span class="sxs-lookup"><span data-stu-id="dbaa2-104">Team channels are places where everyone on the team can openly have conversations.</span></span> <span data-ttu-id="dbaa2-105">비공개 채팅은 채팅의 해당 사용자만 볼 수 있으며 채팅에서 공유하는 파일은 비즈니스용 OneDrive에 저장됩니다.</span><span class="sxs-lookup"><span data-stu-id="dbaa2-105">Private chats are only visible to those people in the chat (and files that you share in a chat are stored in OneDrive for Business).</span></span>

<span data-ttu-id="dbaa2-106">사용자가 비공개 채팅에서 파일을 공유할 때 파일은 공유 사용자의 비즈니스용 OneDrive에 저장됩니다.</span><span class="sxs-lookup"><span data-stu-id="dbaa2-106">When users share files in private chats, the file is stored on the sharing user's OneDrive for Business.</span></span> <span data-ttu-id="dbaa2-107">사용자가 기존 비공개 채팅에 추가된 경우 원래 소유자가 파일을 다시 공유하지 않으면 파일에 액세스할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="dbaa2-107">If a user was added to an existing private chat, they won't be able to access the files unless the original owner re-shares the file.</span></span>    

<span data-ttu-id="dbaa2-108">**채널 대화의 경우:**</span><span class="sxs-lookup"><span data-stu-id="dbaa2-108">**For channel conversations:**</span></span>

- <span data-ttu-id="dbaa2-109">[Microsoft Teams에서 파일 공유는](https://docs.microsoft.com/MicrosoftTeams/sharing-files-in-teams) SharePoint 또는 OneDrive에 구성된 설정을 기반으로 합니다.</span><span class="sxs-lookup"><span data-stu-id="dbaa2-109">[Sharing files in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/sharing-files-in-teams) is based on the settings configured in SharePoint or OneDrive.</span></span> 
- <span data-ttu-id="dbaa2-110">팀과 파일 공동 작업을 [검토하여](https://support.office.com/article/Collaborate-on-files-with-your-Team-9b200289-dbac-4823-85bd-628a5c7bb0ae) 조직에서 Teams를 통해 파일을 공유하고 공동 작업하는 방법에 대해 자세히 알아보는 방법을 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="dbaa2-110">Review [Collaborate on files with your Team](https://support.office.com/article/Collaborate-on-files-with-your-Team-9b200289-dbac-4823-85bd-628a5c7bb0ae) to learn more about how Teams allows your organization to share and collaborate on files.</span></span> 
- <span data-ttu-id="dbaa2-111">새 팀 구성원이 파일에 액세스하는 데 지연이 있는 경우 복제가 완료될 수 있도록 지원 티켓을 열기 **전에 최소 4시간을** 기다릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="dbaa2-111">If new team members experience a delay in accessing files, please wait at least **4 hours** before opening a support ticket to allow replication to complete.</span></span> 

<span data-ttu-id="dbaa2-112">사용자가 이전에 팀 채널의 파일 탭을 통해 파일에 액세스할 수 있으며 "이러한 파일을 더 이상 사용할 수 없습니다."라는 오류가 표시될 경우 SharePoint 사이트 또는 문서 라이브러리의 이름을 변경한지 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="dbaa2-112">If users could previously access files via the Files tab on a team channel, and you get a "these files are no longer available" error, check to see if the SharePoint site or document library has been renamed.</span></span> <span data-ttu-id="dbaa2-113">Teams용 SharePoint 사이트 및 문서 라이브러리의 이름 변경은 아직 지원되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="dbaa2-113">Renaming SharePoint sites and document libraries for Teams is not yet supported.</span></span> <span data-ttu-id="dbaa2-114">이 문제를 해결하기 위해 이 팀에 사용되는 팀 사이트를 열고 라이브러리 이름을 다시 "공유 문서"로 변경합니다.</span><span class="sxs-lookup"><span data-stu-id="dbaa2-114">To resolve this issue, open the team site used for this team and rename the library back to “Shared Documents”.</span></span>