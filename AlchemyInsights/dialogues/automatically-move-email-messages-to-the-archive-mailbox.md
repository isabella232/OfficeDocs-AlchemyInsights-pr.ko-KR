---
title: 전자 메일 메시지를 보관 사서함으로 자동 이동
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50522417"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="7b3ee-102">전자 메일 메시지를 보관 사서함으로 자동 이동</span><span class="sxs-lookup"><span data-stu-id="7b3ee-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="7b3ee-103">사용자의 이전 전자 메일을 보관 사서함으로 자동으로 이동하도록 정책을 설정하는 방법에는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="7b3ee-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="7b3ee-104">보안 및 [**&**](https://go.microsoft.com/fwlink/p/?linkid=2077143)데이터 거버넌스  >    >  **보관함으로** 이동하여 보관 사서함이 사용자에 대해 사용하도록 설정되어 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="7b3ee-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="7b3ee-105">그렇지 않은 경우 경고  상자에서 사용, **예를** 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="7b3ee-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="7b3ee-106">Exchange 관리 [**센터로 이동하여 > 관리 > 관리합니다.**](https://go.microsoft.com/fwlink/?linkid=2059104)</span><span class="sxs-lookup"><span data-stu-id="7b3ee-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="7b3ee-107">+ 아이콘을 선택한 다음 **전체 사서함에 자동으로 적용을 선택 합니다.**</span><span class="sxs-lookup"><span data-stu-id="7b3ee-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="7b3ee-108">보존 태그에 이름을 할당하고 **보관함으로 이동을 선택하십시오.**</span><span class="sxs-lookup"><span data-stu-id="7b3ee-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="7b3ee-109">보존 기간에 대해 90일과 같이 원하는 시간을 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="7b3ee-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="7b3ee-110">**저장** 을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="7b3ee-110">Click **Save**.</span></span>
5. <span data-ttu-id="7b3ee-111">이제 보존 정책 만들기: 보존 **정책 을 선택하고** 아이콘을 선택하면 새 정책을 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7b3ee-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="7b3ee-112">보존 정책에 이름을 할당한 다음 클릭한 후 스크롤하여 방금 만든 보존 태그를 찾아 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="7b3ee-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="7b3ee-113">**저장** 을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="7b3ee-113">Click **Save**.</span></span>
7. <span data-ttu-id="7b3ee-114">마지막으로, 사용자의 사서함에 보존 정책을 적용합니다. 여전히 Exchange 관리 센터에서 받는 사람   >  **사서함으로 이동하세요.**</span><span class="sxs-lookup"><span data-stu-id="7b3ee-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="7b3ee-115">정책을 적용할 모든 사용자를 선택한 다음 편집(연필 아이콘)을 선택하십시오. </span><span class="sxs-lookup"><span data-stu-id="7b3ee-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="7b3ee-116">대화 상자에서 사서함 **기능을 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="7b3ee-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="7b3ee-117">보존 **정책에서** 방금 만든 정책을 저장에서 > **적용합니다.**</span><span class="sxs-lookup"><span data-stu-id="7b3ee-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="7b3ee-118">모든 사용자에게 정책을 적용하는 방법에 대한 지침은 사서함에 보존 [정책 적용을 참조하세요.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)</span><span class="sxs-lookup"><span data-stu-id="7b3ee-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>
