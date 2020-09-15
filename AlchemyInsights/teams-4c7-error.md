---
title: 팀 4c7 오류
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
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700209"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="b5e8e-102">Microsoft 팀의 경우 4c7 오류</span><span class="sxs-lookup"><span data-stu-id="b5e8e-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="b5e8e-103">이 오류는 Microsoft 팀이 폼 인증을 필요로 하기 때문에 발생 합니다.</span><span class="sxs-lookup"><span data-stu-id="b5e8e-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="b5e8e-104">AD FS (Active Directory Federation Services)를 배포할 때 기본적으로 인트라넷에 대해 폼 인증을 사용 하도록 설정 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="b5e8e-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="b5e8e-105">Windows 통합 인증이 실패 하면 폼 인증을 사용 하 여 로그인 하 라는 메시지가 표시 됩니다.</span><span class="sxs-lookup"><span data-stu-id="b5e8e-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="b5e8e-106">이 문제를 해결 하려면 Active Directory의 로컬 복사본이 있는 컴퓨터에서 AD FS MMC (Microsoft Management Console) 스냅인을 사용 하 여 폼 인증을 사용 하도록 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="b5e8e-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="b5e8e-107">이렇게 하려면 다음과 같이 하십시오.</span><span class="sxs-lookup"><span data-stu-id="b5e8e-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="b5e8e-108">탐색 창에서 **인증 정책**으로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="b5e8e-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="b5e8e-109">세부 정보 창의 **작업** 아래에서 **전역 기본 인증 편집**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b5e8e-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="b5e8e-110">**인트라넷** 탭에서 **폼 인증**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b5e8e-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="b5e8e-111">확인 또는 **적용** **을** 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="b5e8e-111">Select **OK** (or **Apply**).</span></span>