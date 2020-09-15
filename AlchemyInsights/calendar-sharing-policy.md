---
title: 618 일정 공유 정책
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684236"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="906bf-102">일정을 공유할 때의 정책 오류</span><span class="sxs-lookup"><span data-stu-id="906bf-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="906bf-103">상황에 따라 다음 중 하나를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="906bf-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="906bf-104">원격 PowerShell을 사용 하 여 Exchange Online에 연결 합니다.</span><span class="sxs-lookup"><span data-stu-id="906bf-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="906bf-105">자세한 내용은 [원격 PowerShell을 사용 하 여 Exchange Online에 연결](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="906bf-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="906bf-106">온-프레미스 서버에서 Exchange 관리 셸을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="906bf-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="906bf-107">사용자에 게 할당 된 공유 정책을 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="906bf-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="906bf-108">이렇게 하려면 다음 명령을 실행 하 여 반환 되는 정책을 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="906bf-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="906bf-109">사용자에 대 한 공유 정책을 업데이트 합니다.</span><span class="sxs-lookup"><span data-stu-id="906bf-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="906bf-110">이렇게 하려면 다음과 같이 하십시오.</span><span class="sxs-lookup"><span data-stu-id="906bf-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="906bf-111">Exchange 관리 센터를 엽니다.</span><span class="sxs-lookup"><span data-stu-id="906bf-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="906bf-112">**조직을**클릭 한 다음 **개별 공유**에서 사용자에 게 할당 된 정책을 두 번 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="906bf-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="906bf-113">이 정책은 2 단계에서 반환 된 정책입니다.</span><span class="sxs-lookup"><span data-stu-id="906bf-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="906bf-114">공유 규칙 페이지에서 **공유 하려는 정보 지정**에서 허용할 일정 공유 수준을 선택 합니다. **저장**을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="906bf-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="906bf-115">자세한 내용은 ["정책에서이 수준에 하나 이상의 받는 사람에 게 사용 권한을 부여 하는 것을 허용 하지 않습니다." (사용자가 일정을 공유 하려고 할 때) 오류를](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="906bf-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
