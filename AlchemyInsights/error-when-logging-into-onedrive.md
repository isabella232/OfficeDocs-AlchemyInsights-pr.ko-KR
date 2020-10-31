---
title: OneDrive를 시작할 때 발생 하는 오류 0x8004de40
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
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/30/2020
ms.locfileid: "48815994"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="95f84-102">OneDrive를 시작할 때 발생 하는 오류 0x8004de40</span><span class="sxs-lookup"><span data-stu-id="95f84-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="95f84-103">OneDrive에 로그인 할 때 오류 **0x8004de40** 이 나타나면 회사 또는 학교 도메인에 연결 된 상태에서 컴퓨터를 다시 부팅 합니다.</span><span class="sxs-lookup"><span data-stu-id="95f84-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="95f84-104">다시 부팅 한 후에이 오류가 나타나면 회사 또는 학교 도메인에 연결 되어 있는 동안 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="95f84-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="95f84-105">시작을 클릭 하 고 검색 상자에 **cmd** 또는 **명령 프롬프트**  를 입력 하 고 명령 프롬프트 앱을 마우스 오른쪽 단추로 클릭 한 다음  **관리자 권한으로 실행** 을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="95f84-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator** .</span></span> <span data-ttu-id="95f84-106">관리자 암호나 확인을 묻는 메시지가 표시 되 면 암호를 입력 하거나 **허용** 을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="95f84-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow** .</span></span>  

2. <span data-ttu-id="95f84-107">명령 프롬프트 창에서 **dsregcmd/leave**  를 입력 하 고 명령이 완료 될 때까지 기다립니다.</span><span class="sxs-lookup"><span data-stu-id="95f84-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="95f84-108">그런 다음 **dsregcmd/tjoin** 을 입력 하 고 명령이 완료 될 때까지 기다립니다.</span><span class="sxs-lookup"><span data-stu-id="95f84-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="95f84-109">컴퓨터를 다시 부팅 합니다.</span><span class="sxs-lookup"><span data-stu-id="95f84-109">Reboot your computer.</span></span>
