---
title: 하드 코드된 경로 대신 데이터 디렉터리 변수를 사용하여 Microsoft Edge 수정
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "9003873"
- "6926"
ms.openlocfilehash: 5c40aa1d7f61fbd2842839a5839899af8ab439f2
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49608846"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a><span data-ttu-id="7834d-102">하드 코드된 경로 대신 데이터 디렉터리 변수를 사용하여 Microsoft Edge 수정</span><span class="sxs-lookup"><span data-stu-id="7834d-102">Modify Microsoft Edge by using data directory variables rather than hardcoded paths</span></span>

<span data-ttu-id="7834d-103">예를 들어 Windows에서 프로필 데이터를 기본 위치가 아닌 사용자의 로컬 응용 프로그램 데이터 아래에 저장하려면 **UserDataDir** 정책을 **${local_app_data}\Edge\Profile로** 설정하십시오.</span><span class="sxs-lookup"><span data-stu-id="7834d-103">For example, on Windows, to store the profile data under a user's local application data rather than in the default location, set the **UserDataDir** policy to **${local_app_data}\Edge\Profile**.</span></span> 

<span data-ttu-id="7834d-104">자세한 내용은 Microsoft Edge 사용자 데이터 디렉터리 변수 [만들기를 참조하십시오.](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars)</span><span class="sxs-lookup"><span data-stu-id="7834d-104">To learn more, see [Create Microsoft Edge user data directory variables](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars).</span></span>