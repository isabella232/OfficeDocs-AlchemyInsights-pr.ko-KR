---
title: 보관 사서함 사용
ms.author: markjjo
author: markjjo
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "307"
- "3100008"
ms.assetid: e1a5fab7-d3a5-4d4c-8ee2-0edf4ec9b76b
ms.openlocfilehash: 3e20eaf8dec85454ce5a67e1b21292b2a33ebb1d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47811711"
---
# <a name="enable-an-archive-mailbox"></a><span data-ttu-id="1fc3d-102">보관 사서함 사용</span><span class="sxs-lookup"><span data-stu-id="1fc3d-102">Enable an archive mailbox</span></span>

<span data-ttu-id="1fc3d-103">자동 검사를 실행 하 여 보관 사서함을 구성할 수 있도록 하려면이 페이지 맨 위에 있는 뒤로 단추 <----해당 계정의 전자 메일 주소를 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="1fc3d-103">If you want us to run automated checks to ensure an archive mailbox can be configured, select the back button <-- at the top of this page, and then enter the email address of the account.</span></span>

<span data-ttu-id="1fc3d-104">Microsoft 365의 보관 사서함 ( *온라인 보관* 또는 원본 *위치 보관*이 라고도 함)은 사용자에 게 추가 전자 메일 저장소를 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="1fc3d-104">Archive mailboxes in Microsoft 365 (also called *Online Archives* or *In-Place Archives*) provide users with additional email storage.</span></span> <span data-ttu-id="1fc3d-105">사용자는 보관 사서함으로 항목을 이동 하거나 복사할 수 있으며, 관리자는 항목을 보관 사서함으로 자동으로 이동 하는 보관 정책을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1fc3d-105">Users can move or copy items to their archive mailbox, and admins can create an archive policy that automatically moves items to archive mailboxes.</span></span>
  
<span data-ttu-id="1fc3d-106">보관 사서함을 만드는 방법은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="1fc3d-106">Here's how to create an archive mailbox:</span></span>
  
1. <span data-ttu-id="1fc3d-107">[https://protection.office.com](https://protection.office.com)으로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="1fc3d-107">Go to [https://protection.office.com](https://protection.office.com).</span></span>

2. <span data-ttu-id="1fc3d-108">관리자 계정을 사용 하 여 Microsoft 365에 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="1fc3d-108">Sign in to Microsoft 365 using your admin account.</span></span>

3. <span data-ttu-id="1fc3d-109">보안 및 준수 센터의 왼쪽 창에서 &amp; **정보 거 버 넌 스** \> **보관**함을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="1fc3d-109">In the left pane of the Security &amp; Compliance Center, select **Information governance** \> **Archive**.</span></span>

4. <span data-ttu-id="1fc3d-110">보관 사서함을 사용 하도록 설정 하려는 사용자를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="1fc3d-110">Select the user whose archive mailbox you want to enable.</span></span>

5. <span data-ttu-id="1fc3d-111">오른쪽의 세부 정보 창에서 **사용** 을 클릭 한 다음 경고 메시지에서 **예** 를 클릭 하 여 보관 사서함을 사용 하도록 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="1fc3d-111">In the details pane on the right, click **Enable** and then click **Yes** in the warning message to enable the archive mailbox.</span></span>

<span data-ttu-id="1fc3d-112">**Shift** 또는 **Ctrl** 키를 사용 하 여 여러 사용자를 선택한 다음 세부 정보 창에서 **사용** 을 클릭 하 여 보관 사서함을 대량으로 사용 하도록 설정할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1fc3d-112">You can also bulk-enable archive mailboxes by selecting multiple users (using the **Shift** or **Ctrl** keys) and then clicking **Enable** in the details pane.</span></span>
  
### <a name="shared-mailboxes"></a><span data-ttu-id="1fc3d-113">공유 사서함</span><span class="sxs-lookup"><span data-stu-id="1fc3d-113">Shared mailboxes</span></span>

<span data-ttu-id="1fc3d-114">공유 사서함에 대 한 보관 함을 사용 하도록 설정 하려면 exchange online 계획 2 라이선스 또는 교환 라이선스가 있는 exchange online 계획 1 라이선스가 필요 합니다.</span><span class="sxs-lookup"><span data-stu-id="1fc3d-114">To enable the archive for a shared mailbox, an Exchange Online Plan 2 license or an Exchange Online Plan 1 license with an Exchange Online Archiving license is required.</span></span>  

<span data-ttu-id="1fc3d-115">공유 사서함에 대 한 보관 함을 사용 하도록 설정 하려면 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="1fc3d-115">To enable the archive for a shared mailbox:</span></span>

1. <span data-ttu-id="1fc3d-116">[Exchange 관리 센터로](https://outlook.office365.com/ecp) 이동 하 여 관리자 계정을 사용 하 여 로그인 합니다.</span><span class="sxs-lookup"><span data-stu-id="1fc3d-116">Go to the [Exchange admin center](https://outlook.office365.com/ecp) and sign in using your admin account.</span></span>

2. <span data-ttu-id="1fc3d-117">공유 되는 **받는 사람**으로 이동  >  **Shared**합니다.</span><span class="sxs-lookup"><span data-stu-id="1fc3d-117">Go to **Recipients** > **Shared**.</span></span>

3. <span data-ttu-id="1fc3d-118">공유 사서함을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="1fc3d-118">Select the shared mailbox.</span></span>

4. <span data-ttu-id="1fc3d-119">오른쪽의 세부 정보 창에서 원본 **위치 보관 함**아래에서 **사용**을 클릭 한 다음 **예** 를 클릭 하 여 보관 사서함을 사용 하도록 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="1fc3d-119">In the details pane on the right, under **In-Place Archive**, click **Enable**, and then click **Yes** to enable the archive mailbox.</span></span>

<span data-ttu-id="1fc3d-120">자세한 내용은 다음을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1fc3d-120">For more information, see:</span></span>
  
- [<span data-ttu-id="1fc3d-121">보관 사서함 사용</span><span class="sxs-lookup"><span data-stu-id="1fc3d-121">Enable archive mailboxes</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes)

- [<span data-ttu-id="1fc3d-122">보관 및 삭제 정책 설정</span><span class="sxs-lookup"><span data-stu-id="1fc3d-122">Set up an archive and deletion policy</span></span>](https://docs.microsoft.com//office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes)
