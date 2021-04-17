---
title: 전자 메일의 이벤트 문제 해결
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834845"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="e1e87-102">전자 메일의 이벤트 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e1e87-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="e1e87-103">사서함에 대해 이 기능을 사용하도록 설정되었는지 확인합니다. **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="e1e87-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="e1e87-104">그런 다음 '전자 메일의 이벤트' 로그 **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile** 을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="e1e87-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="e1e87-105">'전자 메일의 이벤트' 로그에서 사서함의 항목과 일치하는 InternetMessageId를 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="e1e87-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="e1e87-106">TrustScore는 항목이 추가되는지 여부를 결정합니다.</span><span class="sxs-lookup"><span data-stu-id="e1e87-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="e1e87-107">TrustScore = "신뢰됨"인 경우에만 이벤트를 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e1e87-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="e1e87-108">TrustScore는 메시지 머리글에 있는 SPF, Dkim 또는 Dmarc 속성에 따라 결정됩니다.</span><span class="sxs-lookup"><span data-stu-id="e1e87-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="e1e87-109">이러한 속성을 보려면 다음을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="e1e87-109">To view these properties:</span></span>

<span data-ttu-id="e1e87-110">**데스크톱 Outlook**</span><span class="sxs-lookup"><span data-stu-id="e1e87-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="e1e87-111">항목 열기</span><span class="sxs-lookup"><span data-stu-id="e1e87-111">Open the item</span></span>
- <span data-ttu-id="e1e87-112">파일 -> 속성 -> 인터넷 머리글</span><span class="sxs-lookup"><span data-stu-id="e1e87-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="e1e87-113">또는</span><span class="sxs-lookup"><span data-stu-id="e1e87-113">or</span></span>

<span data-ttu-id="e1e87-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="e1e87-114">**MFCMapi**</span></span>

- <span data-ttu-id="e1e87-115">받은 편지함에서 해당 항목으로 이동</span><span class="sxs-lookup"><span data-stu-id="e1e87-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="e1e87-116">PR_TRANSPORT_MESSAGE_HEADERS_W 확인</span><span class="sxs-lookup"><span data-stu-id="e1e87-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="e1e87-117">이러한 속성은 전송과 라우팅을 수행하는 동안 결정되고 기록됩니다.</span><span class="sxs-lookup"><span data-stu-id="e1e87-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="e1e87-118">추가 문제 해결을 위해 SPF, DKIM 및/또는 DMARC의 오류에 대한 전송 지원을 추가해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e1e87-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>