---
title: 1332 OWA-사서함에 대 한 받은 편지함 규칙이 실행 되 고 있지 않음
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 9abdcdcb33d39b8b9fe2df80f0c15a8b55e465fd
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44576566"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="e1753-102">받은 편지함 규칙이 예상 대로 작동 하지 않음</span><span class="sxs-lookup"><span data-stu-id="e1753-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="e1753-103">웹용 Outlook에서 다음 설정을 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="e1753-103">Verify the following settings in Outlook on the web:</span></span>

- <span data-ttu-id="e1753-104">받은 편지함 규칙을 한 번에 하나씩 자동으로 사용 하 여 메시지를 리디렉션하고 전달 하거나 회신할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e1753-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="e1753-105">리디렉션 규칙 (받은 편지함 규칙 또는 전송 규칙이 라고도 하는 메일 흐름 규칙)은 최대 10 개의 전달 받는 사람을 메시지에 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e1753-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="e1753-106">자세한 내용은 [저널, 전송 및 받은 편지함 규칙 제한을](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="e1753-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="e1753-107">받은 편지함 규칙은 대체 저널링 사서함에서 작동 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="e1753-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="e1753-108">대체 저널링 사서함에 대 한 자세한 내용은 [대체 저널링 사서함](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)을 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="e1753-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="e1753-109">이러한 문제를 해결 하려면 [Kb(52829319](https://support.microsoft.com/kb/2829319)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="e1753-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="e1753-110">이전 문제가 적용 되지 않으면 Microsoft 지원으로 문제를 에스컬레이션 하기 전에 받은 편지함 규칙 진단 보고서를 실행 합니다.</span><span class="sxs-lookup"><span data-stu-id="e1753-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="e1753-111">웹용 Outlook에서 사서함을 열고</span><span class="sxs-lookup"><span data-stu-id="e1753-111">Open the mailbox in Outlook on the web, and click</span></span> <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 <span data-ttu-id="e1753-112">**설정**  >  **모든 Outlook 설정 보기**  >  **메일**  >  **규칙**입니다.</span><span class="sxs-lookup"><span data-stu-id="e1753-112">**Settings** > **View all Outlook Settings** > **Mail** > **Rules**.</span></span>

2. <span data-ttu-id="e1753-113">페이지 맨 아래에서 **규칙이 작동 하지 않으면 여기를 클릭 하 여 진단 보고서를 생성**합니다.</span><span class="sxs-lookup"><span data-stu-id="e1753-113">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
