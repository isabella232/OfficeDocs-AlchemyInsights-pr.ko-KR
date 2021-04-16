---
title: Teams 4c7 오류
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
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786675"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="0ddf5-102">Microsoft Teams의 4c7 오류</span><span class="sxs-lookup"><span data-stu-id="0ddf5-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="0ddf5-103">이 오류는 Microsoft Teams에 폼 인증이 필요하기 때문에 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="0ddf5-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="0ddf5-104">AD FS(Active Directory Federation Services)를 배포할 때 기본적으로 인트라넷에 대해 폼 인증을 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="0ddf5-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="0ddf5-105">Windows 통합 인증이 실패하면 폼 인증을 사용하여 로그인하라는 메시지가 표시될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0ddf5-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="0ddf5-106">이 문제를 해결하려면 Active Directory의 로컬 복사본이 있는 컴퓨터에서 AD FS MMC(Microsoft Management Console) 스냅인을 사용하여 폼 인증을 사용하도록 설정하십시오.</span><span class="sxs-lookup"><span data-stu-id="0ddf5-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="0ddf5-107">이렇게 하려면 다음과 같이 하십시오.</span><span class="sxs-lookup"><span data-stu-id="0ddf5-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="0ddf5-108">탐색 창에서 인증 **정책으로 이동합니다.**</span><span class="sxs-lookup"><span data-stu-id="0ddf5-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="0ddf5-109">세부 **정보** 창의 작업에서 전역 기본 인증 **편집을 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="0ddf5-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="0ddf5-110">**인트라넷 탭에서** 폼 **인증을 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="0ddf5-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="0ddf5-111">**확인(또는** **적용)을 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="0ddf5-111">Select **OK** (or **Apply**).</span></span>