---
title: 0x8004de40 시작 시 발생하는 오류 발생
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
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813658"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="e308d-102">0x8004de40 시작 시 발생하는 오류 발생</span><span class="sxs-lookup"><span data-stu-id="e308d-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="e308d-103">OneDrive에 **로그인할 0x8004de40** 오류가 발생하면 직장 또는 학교 도메인에 연결된 동안 컴퓨터를 다시 시작하십시오.</span><span class="sxs-lookup"><span data-stu-id="e308d-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="e308d-104">다시 부팅한 후 이 오류가 표시되면 직장 또는 학교 도메인에 연결된 동안 시도해 보아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="e308d-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="e308d-105">시작을 클릭하고 검색  상자에 **cmd** 또는 명령 프롬프트를 입력하고 명령 프롬프트 앱을 마우스 오른쪽 단추로 클릭한 다음 **관리자 권한으로 실행을 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="e308d-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator**.</span></span> <span data-ttu-id="e308d-106">관리자 암호를 입력하거나 확인 메시지를 표시하는 경우 암호를 입력하거나 허용 을 **클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="e308d-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow**.</span></span>  

2. <span data-ttu-id="e308d-107">명령 프롬프트 창에 **dsregcmd /leave를**  입력하고 명령이 완료될 때까지 기다립니다.</span><span class="sxs-lookup"><span data-stu-id="e308d-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="e308d-108">그런 다음 **dsregcmd /join을 입력하고** 명령이 완료될 때까지 기다릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e308d-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="e308d-109">컴퓨터를 다시 시작하십시오.</span><span class="sxs-lookup"><span data-stu-id="e308d-109">Reboot your computer.</span></span>
