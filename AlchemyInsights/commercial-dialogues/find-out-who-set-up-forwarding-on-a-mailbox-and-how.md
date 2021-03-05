---
title: 사서함에 대해 전달을 설정하는 사람 및 방법 확인
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464870"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="9bc3e-102">사서함에 대해 전달을 설정하는 사람 및 방법 확인</span><span class="sxs-lookup"><span data-stu-id="9bc3e-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="9bc3e-103">외부 전달이 사서함에 설정된 경우 활동은 사서함 cmdlet의 일부로 Set-Mailbox 감사됩니다.</span><span class="sxs-lookup"><span data-stu-id="9bc3e-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="9bc3e-104">감사 로그에서 활동을 찾는 방법에는 다음이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9bc3e-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="9bc3e-105">[Office 365 보안](https://go.microsoft.com/fwlink/p/?linkid=2077143)및 준수 & 로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="9bc3e-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="9bc3e-106">감사 **로그** >  **검색 검색을 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="9bc3e-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="9bc3e-107">감사를 켜야 하는 알림이 표시된 경우 지금 진행하여 켜야 합니다.</span><span class="sxs-lookup"><span data-stu-id="9bc3e-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="9bc3e-108">이 기능을 설정하지 않은 경우 검색 결과에서 이전 날짜의 데이터를 끌 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="9bc3e-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="9bc3e-109">활동 **필드가** 모든 활동에 대한 결과 표시(기본값)로 **설정되어** 있는지 확인</span><span class="sxs-lookup"><span data-stu-id="9bc3e-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="9bc3e-110">날짜 범위를 지정합니다.</span><span class="sxs-lookup"><span data-stu-id="9bc3e-110">Specify the date range.</span></span> <span data-ttu-id="9bc3e-111">사용자 이름을 지정할 필요가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="9bc3e-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="9bc3e-112">검색 **을 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="9bc3e-112">Select **Search**.</span></span> <span data-ttu-id="9bc3e-113">활동은 결과 아래에 **표시됩니다.**</span><span class="sxs-lookup"><span data-stu-id="9bc3e-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="9bc3e-114">필터 **결과 를** 선택한 다음 활동 필터 필드에 **Set-mailbox를** 입력합니다. </span><span class="sxs-lookup"><span data-stu-id="9bc3e-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="9bc3e-115">그러면 모든 **Set-Mailbox 활동이 반환됩니다.**</span><span class="sxs-lookup"><span data-stu-id="9bc3e-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="9bc3e-116">세부 정보를 확인하려면 활동을 선택한 다음 추가 정보 **를 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="9bc3e-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="9bc3e-117">매개 **변수에서** 사서함에 설정된 전달 전자 메일 주소를 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9bc3e-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="9bc3e-118">**UserID는** 사서함에 외부 전달을 설정한 사용자를 나타내며,</span><span class="sxs-lookup"><span data-stu-id="9bc3e-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="9bc3e-119">자세한 내용은 [Office 365](https://go.microsoft.com/fwlink/?linkid=2103944)감사 로그 검색을 참조하여 일반적인 시나리오 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="9bc3e-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>