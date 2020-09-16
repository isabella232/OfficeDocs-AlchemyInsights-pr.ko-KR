---
title: OneDrive에서 0x8004de40 오류 수정
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745136"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="b4b50-102">OneDrive에서 0x8004de40 오류 수정</span><span class="sxs-lookup"><span data-stu-id="b4b50-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="b4b50-103">OneDrive와 함께 0x8004de40 오류가 표시 되는 경우:</span><span class="sxs-lookup"><span data-stu-id="b4b50-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="b4b50-104">Acitve 디렉터리 도메인에 연결 된 상태에서 영향을 받는 컴퓨터를 다시 부팅 합니다.</span><span class="sxs-lookup"><span data-stu-id="b4b50-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="b4b50-105">다시 부팅 해도 문제가 해결 되지 않으면 Azure AD에서 디바이스를 가입 하지 않고 참가 시킵니다.</span><span class="sxs-lookup"><span data-stu-id="b4b50-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="b4b50-106">**참고**: 다음 단계를 수행 하는 동안 회사 네트워크에 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="b4b50-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="b4b50-107">회사 인프라 (예: 여행 중)에 연결할 수 없는 경우에는이 단계를 수행 하지 마십시오.</span><span class="sxs-lookup"><span data-stu-id="b4b50-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="b4b50-108">승격된 명령 프롬프트를 엽니다.</span><span class="sxs-lookup"><span data-stu-id="b4b50-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="b4b50-109">관리자 권한 명령 프롬프트를 열려면- **Start**를 클릭 하 고 **명령 프롬프트**를 마우스 오른쪽 단추로 클릭 한 다음 **관리자 권한으로 실행**을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="b4b50-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="b4b50-110">*Dsregcmd/leave* 를 입력 하 고 enter 키 **를 누릅니다.**</span><span class="sxs-lookup"><span data-stu-id="b4b50-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="b4b50-111">완료 되 면 *dsregcmd/join* 을 입력 하 **고 enter 키를 누릅니다.**</span><span class="sxs-lookup"><span data-stu-id="b4b50-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="b4b50-112">완료 되 면 명령 프롬프트를 닫습니다.</span><span class="sxs-lookup"><span data-stu-id="b4b50-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="b4b50-113">컴퓨터를 다시 부팅 하 고 OneDrive에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="b4b50-113">Reboot the computer, and log into OneDrive.</span></span>