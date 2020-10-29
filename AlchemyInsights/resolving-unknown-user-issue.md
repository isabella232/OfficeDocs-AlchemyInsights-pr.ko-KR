---
title: 팀 채팅에서 알 수 없는 사용자의 문제 해결
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003807"
- "6809"
ms.openlocfilehash: 523c11cb9d5c4696703c67c2a6b3184f5d12f8e7
ms.sourcegitcommit: d151b09064df3fb573ae07a387a08d98a9553b9b
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/28/2020
ms.locfileid: "48785622"
---
# <a name="resolving-issue-with-unknown-user-in-teams-chat"></a><span data-ttu-id="c62d1-102">팀 채팅에서 "알 수 없는 사용자"의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="c62d1-102">Resolving issue with "Unknown User" in Teams Chat</span></span>

<span data-ttu-id="c62d1-103">제거 된 사용자는 때때로 "알 수 없는 사용자"로 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="c62d1-103">At times, a removed user will appear as "Unknown User".</span></span> <span data-ttu-id="c62d1-104">이는 [알려진 문제](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/removed-user-appears-as-unknown)입니다.</span><span class="sxs-lookup"><span data-stu-id="c62d1-104">This is a [known issue](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/removed-user-appears-as-unknown).</span></span>

<span data-ttu-id="c62d1-105">팀 대화방에서 "알 수 없는 사용자"로 표시 되는 사용자를 명확 하 게 확인 하려면 캐시를 지워 보십시오.</span><span class="sxs-lookup"><span data-stu-id="c62d1-105">If you are persistently seeing users showing as "Unknown User" in Teams chats, try and clear the cache:</span></span>

1.  <span data-ttu-id="c62d1-106">작업 표시줄에서 팀 아이콘을 마우스 오른쪽 단추로 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="c62d1-106">Right-click the Teams icon in the taskbar.</span></span> <span data-ttu-id="c62d1-107">**종료** 를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="c62d1-107">Click  **Quit** .</span></span>
2.  <span data-ttu-id="c62d1-108">컴퓨터에서 %appdata%\Microsoft\teams\ folder로 이동하고 디렉터리의 모든 파일을 삭제합니다.</span><span class="sxs-lookup"><span data-stu-id="c62d1-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>

<span data-ttu-id="c62d1-109">익명 사용자가 로비에서 대기 하도록 하 여 모임에 참가 하지 못하도록 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c62d1-109">You can prevent anonymous users from joining meetings by ensuring that they wait in the lobby.</span></span> <span data-ttu-id="c62d1-110">자세한 내용은 [팀 모임에 대 한 참가자 설정 변경을](https://support.microsoft.com/office/change-participant-settings-for-a-teams-meeting-53261366-dbd5-45f9-aae9-a70e6354f88e)참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="c62d1-110">For more information, see [Change participant settings for a Teams meeting](https://support.microsoft.com/office/change-participant-settings-for-a-teams-meeting-53261366-dbd5-45f9-aae9-a70e6354f88e).</span></span>
