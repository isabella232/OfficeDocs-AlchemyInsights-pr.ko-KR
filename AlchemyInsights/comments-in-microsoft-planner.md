---
title: Microsoft Planner의 메모
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
- "9001717"
- "3810"
ms.openlocfilehash: 09385fd0235939d01e0baf141362cb8b76910682
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817646"
---
# <a name="comments-in-microsoft-planner"></a><span data-ttu-id="78046-102">Microsoft Planner의 메모</span><span class="sxs-lookup"><span data-stu-id="78046-102">Comments in Microsoft Planner</span></span>

<span data-ttu-id="78046-103">계획의 작업에 대한 메모는 계획에 연결된 Microsofte 365 그룹의 Exchange Online 사서함에 저장됩니다.</span><span class="sxs-lookup"><span data-stu-id="78046-103">Comments for tasks within a plan are stored in the Exchange Online mailbox for the Microsoft 365 Group associated with the plan.</span></span>  <span data-ttu-id="78046-104">작업에 대한 메모를 게시하면 그룹 받은 편지함으로 전자 메일 알림이 전송되고 해당 작업과 관련된 이후의 모든 의견에 대해 전자 메일을 받게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="78046-104">When you post a comment on a task, an email notification is sent to the group inbox, and you will receive an email for each subsequent comment made on that task.</span></span>

<span data-ttu-id="78046-105">다음은 메모와 관련된 몇 가지 일반적인 문제에 대한 답변입니다.</span><span class="sxs-lookup"><span data-stu-id="78046-105">Here are some answers to common issues related to comments:</span></span>

- <span data-ttu-id="78046-106">**사용자가 전자 메일을 받지 못함** - 이 계획을 소유한 그룹의 그룹 받은 편지함으로 의견이 전송됩니다.</span><span class="sxs-lookup"><span data-stu-id="78046-106">**Users are not receiving emails** - Comments are sent to the group inbox for the group the plan belongs to.</span></span> <span data-ttu-id="78046-107">사용자가 그룹 전자 메일을 받으려면 그룹 대화를 구성원의 받은 편지함으로 보내도록 그룹을 구성해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="78046-107">For a user to receive group emails, the group should be configured to send group conversations to member's inboxes.</span></span>

- <span data-ttu-id="78046-108">**의견이 저장되지 않음** - 의견을 추가하는 사용자에게 Microsoft 365 그룹으로 전자 메일을 보낼 수 있는 권한이 없습니다.</span><span class="sxs-lookup"><span data-stu-id="78046-108">**Comments are not getting saved** -  The user adding the comment does not have permission to send email to the Microsoft 365 group.</span></span> <span data-ttu-id="78046-109">이 시나리오에 대한 자세한 내용은 [Microsoft Planner가 작동하는 방식](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="78046-109">Read [How Microsoft Planner Works](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) for more information about this scenario.</span></span>

- <span data-ttu-id="78046-110">**더 이상 액세스할 수 없음** 오류가 표시되거나 **게스트 사용자는 메모를 추가할 수 없음** 오류 - 그룹 받은 편지함에 전자 메일을 보낼 수 없는 게스트 사용자에게 이 메시지가 표시될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="78046-110">The error **You no longer have access** is displayed, or **guest users are unable to add comments** - Guest users who cannot send e-mail to the group inbox may see this message.</span></span> <span data-ttu-id="78046-111">오류를 해결하려면 게스트 사용자에게 유효한 전자 메일 주소가 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="78046-111">To resolve, ensure that the guest user has a valid e-mail address.</span></span>

- <span data-ttu-id="78046-112">**삭제한 사용자가 전자 메일을 받음** - 사용자가 계획에서 제거되기 전에 작업에 관한 메모를 남기면 전자 메일 스레드에 해당 작업에 관한 각 의견에서 사용자가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="78046-112">**Removed users are getting emails** -  If a user comments on a task prior to being removed from the plan, the email thread includes the user for each comment made on the task.</span></span>

<span data-ttu-id="78046-113">Microsoft Planner의 메모에 대한 자세한 내용은 [Microsoft Planner가 작동하는 방식](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) 및 [Microsoft Planner의 작업 관련 메모](https://support.microsoft.com/office/fd4aedde-7785-4cd0-96ee-122fbc9140e1)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="78046-113">For detailed information on comments with Microsoft Planner, see [how Microsoft Planner works](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736) and [Comment on tasks in Microsoft Planner](https://support.microsoft.com/office/fd4aedde-7785-4cd0-96ee-122fbc9140e1).</span></span>
