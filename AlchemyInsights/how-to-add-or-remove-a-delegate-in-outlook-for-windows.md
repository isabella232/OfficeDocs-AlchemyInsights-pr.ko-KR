---
title: Windows용 Outlook에서 대리인을 추가하거나 제거하는 방법
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571912"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a><span data-ttu-id="0034d-102">Windows용 Outlook에서 대리인을 추가하거나 제거하는 방법</span><span class="sxs-lookup"><span data-stu-id="0034d-102">How to add or remove a Delegate in Outlook for Windows</span></span>

<span data-ttu-id="0034d-103">Windows용 Outlook에서 대리인을 추가하는 방법:</span><span class="sxs-lookup"><span data-stu-id="0034d-103">To add a Delegate in Outlook for Windows:</span></span> 

1. <span data-ttu-id="0034d-104">파일 탭 **File** 다음에 오는 계정 설정을 **클릭한** 다음 액세스 위임을 **선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="0034d-104">Click on the **File** tab followed by **Account Settings**, and then choose **Delegate Access**.</span></span>
2. <span data-ttu-id="0034d-105">추가를 **클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="0034d-105">Click on **Add**.</span></span> <span data-ttu-id="0034d-106">**Add가** 나타나지 않는 경우 Outlook과 Exchange 간에 활성 연결이 존재하지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0034d-106">If **Add** doesn’t appear, an active connection might not exist between Outlook and Exchange.</span></span> <span data-ttu-id="0034d-107">Outlook 상태 표시줄에 연결 상태가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="0034d-107">The Outlook status bar displays the connection status.</span></span>
3. <span data-ttu-id="0034d-108">대리인으로 지정하려는 사람의 이름을 입력하거나 검색 결과 목록에서 이름을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="0034d-108">Type the name of the person you want to designate as your delegate, or search and choose the name in the search results list.</span></span>

    > [!NOTE]
    > <span data-ttu-id="0034d-109">대리인은 조직의 Exchange GAL(전체 주소 목록)에 있는 사람 되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="0034d-109">The delegate must be a person in your organization's Exchange Global Address List (GAL).</span></span>
4. <span data-ttu-id="0034d-110">추가를 **클릭한** 다음 확인을 **클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="0034d-110">Click on **Add** followed by **OK**.</span></span>
5. <span data-ttu-id="0034d-111">사용 권한 **위임** 대화 상자에서 기본 사용 권한 설정을 적용하거나 Exchange 폴더에 대한 사용자 지정 액세스 수준을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="0034d-111">In the **Delegate Permissions** dialog box, accept the default permission settings or select custom access levels for Exchange folders.</span></span>

    - <span data-ttu-id="0034d-112">대리인이 모임 요청 및 응답에서만 작업할 수 있는 권한이 필요한 경우 **대리인과** 같은 기본 사용 권한 설정은 나에게 전송된 모임 관련 메시지의 복사본을 수신하는 것으로 충분합니다.</span><span class="sxs-lookup"><span data-stu-id="0034d-112">If a delegate needs permission to work only with meeting requests and responses, the default permission settings such as **Delegate receives copies of meeting-related messages sent to me** are sufficient.</span></span> <span data-ttu-id="0034d-113">받은 편지함 사용 권한 **설정은** 없음으로 설정할 수 **있습니다.**</span><span class="sxs-lookup"><span data-stu-id="0034d-113">You can leave the **Inbox** permission setting at **None**.</span></span> <span data-ttu-id="0034d-114">모임 요청 및 응답은 대리인의 받은 편지함으로 직접 이동됩니다.</span><span class="sxs-lookup"><span data-stu-id="0034d-114">Meeting requests and responses will go directly to the delegate's inbox.</span></span>

    > [!NOTE]
    > <span data-ttu-id="0034d-115">기본적으로 대리인에게 일정 폴더에 대한 편집기(항목을 읽고 **만들고** 수정할 **수** 있습니다)가 부여됩니다.</span><span class="sxs-lookup"><span data-stu-id="0034d-115">By default, the delegate is granted **Editor (can read, create, and modify items)** permission to your **Calendar** folder.</span></span> <span data-ttu-id="0034d-116">대리인이 사용자 대신 모임에 응답하면 일정 폴더에 자동으로 **추가됩니다.**</span><span class="sxs-lookup"><span data-stu-id="0034d-116">When the delegate responds to a meeting on your behalf, it is automatically added to your **Calendar** folder.</span></span>

5. <span data-ttu-id="0034d-117">대리인에게 변경된 사용 권한을 알리는 메시지를 보내기 **Automatically send a message to delegate summarizing these permissions** 위해 이러한 사용 권한 요약을 위임할 메시지 자동 보내기 확인란을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="0034d-117">To send a message to notify the delegate of the changed permissions, select the **Automatically send a message to delegate summarizing these permissions** check box.</span></span>
6. <span data-ttu-id="0034d-118">원하는 경우 **대리인을 선택하면** 내 개인 항목 확인란을 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0034d-118">If you want, select the **Delegate can see my private items** check box.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="0034d-119">이 설정은 모든 Exchange 폴더에 영향을 미치게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="0034d-119">This setting affects all Exchange folders.</span></span> <span data-ttu-id="0034d-120">여기에는 모든 메일, 연락처, 일정, 작업, 메모 및 업무 일지 폴더가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="0034d-120">This includes all Mail, Contacts, Calendar, Tasks, Notes, and Journal folders.</span></span> <span data-ttu-id="0034d-121">지정된 폴더에서만 개인 항목에 대한 액세스 권한을 부여할 수 있는 방법은 없습니다.</span><span class="sxs-lookup"><span data-stu-id="0034d-121">There is no way to grant access to private items in only specified folders.</span></span>

7. <span data-ttu-id="0034d-122">**확인** 을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="0034d-122">Choose **OK**.</span></span>

    > [!NOTE]
    >
    > - <span data-ttu-id="0034d-123">대신 보내기 권한이 있는 메시지에는 대리인과 보낸 사람 옆에 있는 사용자 이름이 **모두 포함됩니다.**</span><span class="sxs-lookup"><span data-stu-id="0034d-123">Messages sent with Send on Behalf permissions include both the delegate's and your names next to **From**.</span></span> <span data-ttu-id="0034d-124">다른 사람 이름으로 보내기 권한으로 메시지를 보내면 이름만 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="0034d-124">When a message is sent with Send As permissions, only your name appears.</span></span>
    > - <span data-ttu-id="0034d-125">대리인으로 다른 사람을 추가하고 나면 Exchange 사서함을 Outlook 프로필에 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="0034d-125">Once you add someone as a delegate, they can add your Exchange mailbox to their Outlook profile.</span></span> <span data-ttu-id="0034d-126">자세한 내용은 다른 사람의 메일 및 일정 항목 관리 [항목을 참조하세요.](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5)</span><span class="sxs-lookup"><span data-stu-id="0034d-126">For instructions, see [Manage another person's mail and calendar items](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span></span>

<span data-ttu-id="0034d-127">Windows용 Outlook에서 대리인을 제거하려면</span><span class="sxs-lookup"><span data-stu-id="0034d-127">To remove a Delegate in Outlook for Windows:</span></span>

1. <span data-ttu-id="0034d-128">파일 **탭을** 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="0034d-128">Click on the **File** tab.</span></span>
2. <span data-ttu-id="0034d-129">계정 설정을 **클릭한 다음** 액세스 **위임합니다.**</span><span class="sxs-lookup"><span data-stu-id="0034d-129">Click on **Account Settings** followed by **Delegate Access**.</span></span>
3. <span data-ttu-id="0034d-130">사용 권한을 변경할 대리인의 이름을 선택한 다음 제거를 클릭한 다음 확인을 **클릭합니다.** **Remove**</span><span class="sxs-lookup"><span data-stu-id="0034d-130">Choose the name of the delegate for whom you want to change permissions, and then click on **Remove** followed by **OK**.</span></span>
