---
title: 공유 정책을 만들어 사용자가 조직 외부의 사용자와 일정을 공유할 수 있습니다.
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 9ece122e0905d1afeb26e50fa0a5e049eee5c09d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806729"
---
# <a name="create-a-sharing-policy-to-allow-your-users-to-share-their-calendar-with-people-outside-your-organization"></a><span data-ttu-id="26f55-102">공유 정책을 만들어 사용자가 조직 외부의 사용자와 일정을 공유할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="26f55-102">Create a Sharing Policy to allow your users to share their calendar with people outside your organization</span></span>

1. <span data-ttu-id="26f55-103">Office 365 관리 센터 대시보드에서 **관리** > **Exchange**로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="26f55-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="26f55-104">**조직** > **공유**로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="26f55-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="26f55-105">목록 보기의 **개별 공유**에서 **새로 만들기**를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="26f55-105">In the list view, under **Individual Sharing**, click **New** .</span></span>
4. <span data-ttu-id="26f55-106">**새 공유 정책**의 **정책 이름** 상자에 공유 정책의 이름을 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="26f55-106">In **new sharing policy**, type a friendly name for the sharing policy in the **Policy name** box.</span></span>
5. <span data-ttu-id="26f55-107">**추가**를 클릭하여 정책의 공유 규칙을 정의합니다.</span><span class="sxs-lookup"><span data-stu-id="26f55-107">Click **Add**  to define the sharing rules for the policy.</span></span>
6. <span data-ttu-id="26f55-108">**공유 규칙**에서 다음 옵션 중 하나를 선택하여 공유할 도메인을 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="26f55-108">In **sharing rule**, select one of the following options to specify the domains you want to share with:</span></span>
    - <span data-ttu-id="26f55-109">**모든 도메인과 공유**</span><span class="sxs-lookup"><span data-stu-id="26f55-109">**Sharing with all domains**</span></span>
    - <span data-ttu-id="26f55-110">**특정 도메인과 공유**</span><span class="sxs-lookup"><span data-stu-id="26f55-110">**Sharing with a specific domain**</span></span>
8. <span data-ttu-id="26f55-p101">**특정 도메인과 공유**를 선택하면 공유할 도메인의 이름을 입력합니다. 이 공유 정책에 대해 도메인을 두 개 이상 입력해야 하는 경우 첫 번째 도메인의 설정을 저장한 다음 공유 규칙을 편집하여 도메인을 더 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="26f55-p101">If you select **Sharing with a specific domain**, type the name of the domain you want to share with. If you need to enter more than one domain for this sharing policy, save the settings for the first domain, then edit the sharing rules to add more domains.</span></span>
9. <span data-ttu-id="26f55-113">공유할 수 있는 정보를 지정하려면 **일정 폴더 공유** 확인란을 선택하고 다음 옵션 중 하나를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="26f55-113">To specify the information that can be shared, select the **Share your calendar folder** check box, and then select one of the following options:</span></span>
    - <span data-ttu-id="26f55-114">**약속 있음/없음 일정 정보와 시간만**</span><span class="sxs-lookup"><span data-stu-id="26f55-114">**Calendar free/busy information with time only**</span></span>
    - <span data-ttu-id="26f55-115">**약속 있음/없음 일정 정보와 시간, 제목, 위치**</span><span class="sxs-lookup"><span data-stu-id="26f55-115">**Calendar free/busy information with time, subject, and location**</span></span>
    - <span data-ttu-id="26f55-116">**모든 일정 약속 정보(시간, 주제, 위치 및 제목 포함)**</span><span class="sxs-lookup"><span data-stu-id="26f55-116">**All calendar appointment information, including time, subject, location and title**</span></span>
11. <span data-ttu-id="26f55-117">**저장**을 클릭하여 공유 정책에 대한 규칙을 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="26f55-117">Click **save** to set the rules for the sharing policy.</span></span>
12. <span data-ttu-id="26f55-118">이 공유 정책을 Office 조직의 모든 사용자에 대한 새 기본 공유 정책으로 설정하려면 **이 정책을 내 기본 공유 정책으로 설정** 확인란을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="26f55-118">If you want to set this sharing policy as the new default sharing policy for all users in your organization, select the **Make this policy my default sharing policy** check box.</span></span>
13. <span data-ttu-id="26f55-119">**저장**을 클릭하여 공유 정책을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="26f55-119">Click **save** to create the sharing policy.</span></span>  

<span data-ttu-id="26f55-120">**이 항목에 대한 자세한 내용은 다음을 참조 하세요.**</span><span class="sxs-lookup"><span data-stu-id="26f55-120">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="26f55-121">Exchange Online에서 공유 정책 만들기</span><span class="sxs-lookup"><span data-stu-id="26f55-121">Create a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/create-a-sharing-policy)
- [<span data-ttu-id="26f55-122">Exchange Online의 사서함에 공유 정책 적용</span><span class="sxs-lookup"><span data-stu-id="26f55-122">Apply a sharing policy to mailboxes in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy)
- [<span data-ttu-id="26f55-123">Exchange Online에서 공유 정책 수정, 사용 안 함 또는 제거</span><span class="sxs-lookup"><span data-stu-id="26f55-123">Modify, disable, or remove a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)