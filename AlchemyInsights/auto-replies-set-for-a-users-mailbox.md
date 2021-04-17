---
title: 사서함에 대한 자동 회신 설정
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
- "9000761"
- "3514"
ms.openlocfilehash: 60af581e7fe508ab9644a53873bcd551b3aacff1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820940"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="bd4f5-102">사용자 사서함에 대한 자동 회신 설정</span><span class="sxs-lookup"><span data-stu-id="bd4f5-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="bd4f5-103">**메서드 1**</span><span class="sxs-lookup"><span data-stu-id="bd4f5-103">**Method 1**</span></span>

1. <span data-ttu-id="bd4f5-104">Microsoft 365 포털에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="bd4f5-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="bd4f5-105">**사용자> 활성 사용자**(또는 공유 사서함에서 설정한 경우 **그룹> 공유 사서함**)로 이동하세요.</span><span class="sxs-lookup"><span data-stu-id="bd4f5-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="bd4f5-106">Microsoft Exchange 사서함이 있는 사용자를 선택하세요.</span><span class="sxs-lookup"><span data-stu-id="bd4f5-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="bd4f5-107">바로 가기 메뉴에서 **메일 설정 > 자동 회신**(공유 사서함 인 경우 바로 가기에서 **자동 회신** 클릭)으로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="bd4f5-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="bd4f5-108">**메서드 2**</span><span class="sxs-lookup"><span data-stu-id="bd4f5-108">**Method 2**</span></span>

1. <span data-ttu-id="bd4f5-109">관리자 자격 증명을 사용하여 Microsoft 365 관리 포털에 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="bd4f5-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="bd4f5-110">**관리 센터** 를 확장하고 **Exchange** 를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="bd4f5-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="bd4f5-111">오른쪽 상단에서 그림을 클릭하고 **다른 사용자** 를 클릭한 다음, 변경할 사용자 사서함을 선택하세요.</span><span class="sxs-lookup"><span data-stu-id="bd4f5-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="bd4f5-112">왼쪽에서 **옵션** 을 선택하고 **전자 메일 구성** 을 클릭한 다음 **자동 회신** 을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="bd4f5-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="bd4f5-113">**메서드 3**</span><span class="sxs-lookup"><span data-stu-id="bd4f5-113">**Method 3**</span></span>

<span data-ttu-id="bd4f5-114">Exchange Online PowerShell에서 다음 cmdlet을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="bd4f5-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="bd4f5-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="bd4f5-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="bd4f5-116">이 cmdlet에 대한 자세한 내용은 [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="bd4f5-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
