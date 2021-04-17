---
title: Teams에서 IP video 허용 또는 비활성화
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
- "9002537"
- "5617"
ms.openlocfilehash: 059d7a1ad619e25f14bc6f561693b6fe24355132
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826349"
---
# <a name="teams-allow-or-disable-ip-video"></a><span data-ttu-id="840f5-102">Teams에서 IP video 허용 또는 비활성화</span><span class="sxs-lookup"><span data-stu-id="840f5-102">Teams allow or disable IP video</span></span>

<span data-ttu-id="840f5-103">**모임 정책 변경 또는 생성**</span><span class="sxs-lookup"><span data-stu-id="840f5-103">**Change or create a meeting policy**</span></span>

<span data-ttu-id="840f5-104">모임 정책을 변경하거나 생성하려면 **Microsoft Teams 관리 센터 > 모임 > 모임 정책** 으로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="840f5-104">To change or create a meeting policy, go to the **Microsoft Teams admin center > Meetings > Meeting policies**.</span></span> <span data-ttu-id="840f5-105">목록에서 정책을 선택하거나 **추가** 를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="840f5-105">Select a policy from the list or click **Add**.</span></span> <span data-ttu-id="840f5-106">새 정책을 만들려면 이름과 설명을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="840f5-106">If you're creating a new policy, add a name and description.</span></span> <span data-ttu-id="840f5-107">이름은 특수 문자가 포함될 수 없으며 64자를 초과할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="840f5-107">The name can't contain special characters or be longer than 64 characters.</span></span> <span data-ttu-id="840f5-108">설정을 선택한 다음 **저장** 을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="840f5-108">Choose your settings, and then click **Save**.</span></span>

<span data-ttu-id="840f5-109">예를 들어, 사용자 수가 많고 모임에 필요한 대역폭의 양을 제한하려 한다고 가정해 보겠습니다.</span><span class="sxs-lookup"><span data-stu-id="840f5-109">For example, say you have many users and you want to limit the amount of bandwidth that their meeting would require.</span></span> <span data-ttu-id="840f5-110">"제한된 대역폭"이라는 새 사용자 지정 정책을 만들고 다음 설정을 사용하지 않도록 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="840f5-110">You would create a new custom policy named "Limited bandwidth" and disable the following settings:</span></span>

<span data-ttu-id="840f5-111">**오디오 및 비디오** 에서:</span><span class="sxs-lookup"><span data-stu-id="840f5-111">Under **Audio & video**:</span></span>

- <span data-ttu-id="840f5-112">클라우드 녹음/녹화 허용을 끕니다.</span><span class="sxs-lookup"><span data-stu-id="840f5-112">Turn off Allow cloud recording.</span></span>
- <span data-ttu-id="840f5-113">IP 비디오 허용을 끕니다.</span><span class="sxs-lookup"><span data-stu-id="840f5-113">Turn off Allow IP video.</span></span>

<span data-ttu-id="840f5-114">그 다음 사용자에게 정책을 할당합니다.</span><span class="sxs-lookup"><span data-stu-id="840f5-114">Then assign the policy to the users.</span></span>

<span data-ttu-id="840f5-115">**사용자에게 모임 정책 할당**</span><span class="sxs-lookup"><span data-stu-id="840f5-115">**Assign a meeting policy to users**</span></span>

1. <span data-ttu-id="840f5-116">Microsoft Teams 관리 센터의 왼쪽 탐색 창에서 **사용자** 로 이동한 후 해당 사용자를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="840f5-116">In the left navigation of the Microsoft Teams admin center, go to **Users**, and then click the user.</span></span>
2. <span data-ttu-id="840f5-117">사용자 이름의 왼쪽을 클릭하여 사용자를 선택한 후 **설정 편집** 을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="840f5-117">Select the user by clicking to the left of the user name, and then click **Edit settings**.</span></span>
3. <span data-ttu-id="840f5-118">**모임 정책** 에서 할당하고자 하는 정책을 선택한 뒤 **적용** 을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="840f5-118">Under **Meeting policy**, select the policy you want to assign and then click **Apply**.</span></span>

<span data-ttu-id="840f5-119">자세한 내용은 [Teams에서 모임 정책 관리](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="840f5-119">For more information, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>
