---
title: Teams 채팅에서 공유된 파일에 액세스할 수 없음
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10825"
- "9003042"
ms.openlocfilehash: 5290b1eea907fc5b785c20654d92467a4ed0af04
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505931"
---
# <a name="unable-to-access-files-shared-in-teams-chat"></a><span data-ttu-id="2d0c0-102">Teams 채팅에서 공유된 파일에 액세스할 수 없음</span><span class="sxs-lookup"><span data-stu-id="2d0c0-102">Unable to access files shared in Teams chat</span></span>

<span data-ttu-id="2d0c0-103">Microsoft Teams에서 채팅 창의 사용자가 공유한 파일은 공유 사용자의 OneDrive 사이트에 자동으로 저장됩니다.</span><span class="sxs-lookup"><span data-stu-id="2d0c0-103">In Microsoft Teams, a file shared by a user in a chat window is stored automatically on the sharing user's OneDrive site.</span></span>

<span data-ttu-id="2d0c0-104">다른 사용자가 Teams에서 파일을 열려고 할 때 "이 파일에 액세스할 수 없습니다"라는 오류 메시지가 표시된다면 이 문제는 OneDrive 사이트에서 제한된 액세스 사용자 권한 잠금 모드 기능이 활성화되어 있기 때문에 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="2d0c0-104">When another user tries to open the file in Teams and receives the error message "You don't have access to this file," the issue occurs because the Limited-access user permission lockdown mode feature is activated on your OneDrive site.</span></span>

1. <span data-ttu-id="2d0c0-105">OneDrive 사이트에서 기능을 사용하지 않도록 설정하는 방법에 대한 지침은 [Teams에서 파일을 열 때 발생하는 오류](https://go.microsoft.com/fwlink/?linkid=2155733)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="2d0c0-105">For instructions to disable the feature on the OneDrive site, see [Error when opening a file in Teams](https://go.microsoft.com/fwlink/?linkid=2155733).</span></span>

1. <span data-ttu-id="2d0c0-106">다른 사용자가 OneDrive 사이트에 액세스할 수 있는지 확인하고 [OneDrive 파일 및 폴더 공유](https://go.microsoft.com/fwlink/?linkid=2156017)의 지침에 따라 액세스를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="2d0c0-106">Check whether another user has access to the OneDrive site, and provide access by following the instructions in [Share OneDrive files and folders](https://go.microsoft.com/fwlink/?linkid=2156017).</span></span>