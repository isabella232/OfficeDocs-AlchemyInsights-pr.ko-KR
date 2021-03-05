---
title: 받은 편지함 규칙에 대해 수행되는 이벤트 찾기
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464998"
---
# <a name="find-events-performed-on-inbox-rules"></a><span data-ttu-id="e2854-102">받은 편지함 규칙에 대해 수행되는 이벤트 찾기</span><span class="sxs-lookup"><span data-stu-id="e2854-102">Find events performed on inbox rules</span></span>

<span data-ttu-id="e2854-103">받은 편지함 규칙을 만들거나 변경하거나 삭제하면 이벤트가 감사 로그에 기록됩니다.</span><span class="sxs-lookup"><span data-stu-id="e2854-103">When inbox rules are created, changed, or deleted, the events are recorded in the audit log.</span></span> <span data-ttu-id="e2854-104">검토하는 방법에는 다음이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e2854-104">Here's how to review them:</span></span>

1. <span data-ttu-id="e2854-105">[Office 365 보안](https://go.microsoft.com/fwlink/p/?linkid=2077143)및 준수 & 로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="e2854-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="e2854-106">감사 로그 > 검색을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="e2854-106">Select Search > Audit log search.</span></span>

    > [!NOTE]
    > <span data-ttu-id="e2854-107">감사를 켜야 하는 알림이 표시된 경우 지금 진행하여 켜야 합니다.</span><span class="sxs-lookup"><span data-stu-id="e2854-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="e2854-108">이 기능을 설정하지 않은 경우 검색 결과에서 이전 날짜의 데이터를 끌 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="e2854-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="e2854-109">활동 필드를 선택하고 Exchange 사서함 활동을 찾은 다음 New-InboxRule 받은 편지함 규칙 만들기를 Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="e2854-109">Select the Activities field and find Exchange mailbox activities, and then select New-InboxRule Create inbox rule from Outlook Web App.</span></span> <span data-ttu-id="e2854-110">완료되면 창 외부를 클릭하여 활동 창을 최소화합니다.</span><span class="sxs-lookup"><span data-stu-id="e2854-110">When you're done, click outside of the pane to minimize the Activities pane.</span></span>
1. <span data-ttu-id="e2854-111">날짜 범위를 지정한 다음 사용자 필드에서 조사할 사용자의 사용자 이름을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="e2854-111">Specify the date range, and then in the Users field, select the username for the user you want to investigate.</span></span> <span data-ttu-id="e2854-112">한에 두 개 이상의 사용자를 선택할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e2854-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="e2854-113">검색을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="e2854-113">Select Search.</span></span> <span data-ttu-id="e2854-114">활동은 결과 아래에 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="e2854-114">The activities appear under Results.</span></span>
1. <span data-ttu-id="e2854-115">세부 정보를 확인하려면 활동을 선택한 다음 추가 정보를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="e2854-115">To view details, select an activity, and then select More Information.</span></span> <span data-ttu-id="e2854-116">매개 변수 섹션에서는 규칙의 이름, 조건 집합 및 규칙이 수행할 작업을 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e2854-116">Under the Parameters section you can see the name of the rule, conditions set, and the actions that the rule will take.</span></span>

<span data-ttu-id="e2854-117">자세한 내용은 Office 365 감사 로그 검색을 참조하여 일반적인 시나리오 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="e2854-117">To learn more, see Search the Office 365 audit log to troubleshoot common scenarios.</span></span>