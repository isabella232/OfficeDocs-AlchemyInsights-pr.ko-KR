---
title: 오류:이 컴퓨터의 규칙이 일치 하지 않습니다.
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: ecc1e5ec741cc90c58698991c3a3135f87c39938
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/09/2020
ms.locfileid: "44618019"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="0b225-102">오류:이 컴퓨터의 규칙이 일치 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="0b225-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="0b225-103">이 알려진 문제의 업데이트 된 상태를 확인 하려면 [이 컴퓨터의 규칙이 Microsoft Exchange의 규칙과 일치 하지 않음](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0) 을 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="0b225-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="0b225-104">Outlook 팀은 12928.10000 빌드에 수정 사항을 구현 했습니다.</span><span class="sxs-lookup"><span data-stu-id="0b225-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="0b225-105">수정 프로그램은 이미 초기 참가자에 게 빠르게 전달 되며 6 월 2020 일 후반에 월별 채널로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="0b225-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="0b225-106">빌드를 고정 한 후에는 마지막으로 어떤 규칙을 유지할지 확인 하 라는 메시지가 표시 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0b225-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="0b225-107">메시지가 표시 되 면 서버를 선택한 다음 Outlook에서 다시 이동 하 여 사용 하지 않도록 설정 된 규칙을 다시 사용 하도록 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="0b225-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="0b225-108">수정 프로그램을 사용할 수 있을 때까지 다음 해결 방법을 사용 하십시오.</span><span class="sxs-lookup"><span data-stu-id="0b225-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="0b225-109">**해결 방법**: 최근 보고서에서는 Outlook 데스크톱에서 생성 된 클라이언트 규칙만 있는 문제에 대해 문제가 발생 했습니다.</span><span class="sxs-lookup"><span data-stu-id="0b225-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="0b225-110">계속 해 서 문제가 발생 하면 규칙을 삭제 한 다음이 문제가 해결 될 때까지 OWA (Outlook Web App)에서 규칙을 만들고 편집 하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="0b225-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="0b225-111">규칙을 수동으로 삭제할 수 없으면 outlook을 시작할 때 outlook.exe/cleanrules를 실행 하 여 Outlook 명령을 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0b225-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="0b225-112">이렇게 하면 클라이언트 및 서버 규칙이 모두 삭제 됩니다.</span><span class="sxs-lookup"><span data-stu-id="0b225-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="0b225-113">Outlook 프로필의 모든 계정에 대 한 모든 규칙이 삭제 됩니다.</span><span class="sxs-lookup"><span data-stu-id="0b225-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="0b225-114">이 명령은 명령줄 스위치 문서에 자세히 설명 되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0b225-114">This command is further documented in the Command-line switches  article.</span></span>