---
title: '오류: 이 컴퓨터의 규칙이 일치하지 않습니다.'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782958"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="4d37d-102">오류: 이 컴퓨터의 규칙이 일치하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="4d37d-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="4d37d-103">이 알려진 문제의 업데이트된 상태를 확인하려면 이 컴퓨터의 규칙이 Microsoft Exchange의 규칙과 [일치하지 않습니다.를 참조합니다.](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="4d37d-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="4d37d-104">The Outlook Team has implemented a fix in Build 12928.10000.</span><span class="sxs-lookup"><span data-stu-id="4d37d-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="4d37d-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span><span class="sxs-lookup"><span data-stu-id="4d37d-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="4d37d-106">고정 빌드가 있는 경우 마지막으로 "유지할 규칙"을 묻는 메시지가 표시될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4d37d-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="4d37d-107">메시지가 표시될 때 서버를 선택한 다음 Outlook에서 다시 돌아가 사용하지 않도록 설정한 규칙을 다시 사용하도록 설정하십시오.</span><span class="sxs-lookup"><span data-stu-id="4d37d-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="4d37d-108">수정을 사용할 수 있는 경우 다음 해결 방법을 사용하시기 바랍니다.</span><span class="sxs-lookup"><span data-stu-id="4d37d-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="4d37d-109">**해결 프로그램:** 최근 보고서에서 Outlook 데스크톱에서 클라이언트 규칙만 만든 사용자에 대해 문제가 발생했습니다.</span><span class="sxs-lookup"><span data-stu-id="4d37d-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="4d37d-110">문제가 계속 발생하면 규칙을 삭제한 다음 문제가 해결될 때까지 OWA(Outlook Web App)에서만 규칙을 만들고 편집하는 것이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4d37d-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="4d37d-111">규칙을 수동으로 삭제할 수 없는 경우 /cleanrules /cleanrules를 실행하여 Outlook을 시작할 때 Outlook 명령을 Outlook.exe 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4d37d-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="4d37d-112">그러면 클라이언트 및 서버 규칙이 모두 삭제됩니다.</span><span class="sxs-lookup"><span data-stu-id="4d37d-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="4d37d-113">Outlook 프로필의 모든 계정에 대한 모든 규칙이 삭제됩니다.</span><span class="sxs-lookup"><span data-stu-id="4d37d-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="4d37d-114">이 명령은 명령줄 스위치 문서에 더 설명되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="4d37d-114">This command is further documented in the Command-line switches article.</span></span>

