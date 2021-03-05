---
title: 삭제된 이벤트에 대한 감사 로그 읽기
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
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464858"
---
# <a name="read-the-audit-logs-for-deleted-events"></a><span data-ttu-id="8d74e-102">삭제된 이벤트에 대한 감사 로그 읽기</span><span class="sxs-lookup"><span data-stu-id="8d74e-102">Read the audit logs for deleted events</span></span>

<span data-ttu-id="8d74e-103">이 작업을 하는 방법에는 다음이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8d74e-103">Here's how to do this:</span></span>

1. <span data-ttu-id="8d74e-104">[Office 365 보안](https://go.microsoft.com/fwlink/p/?linkid=2077143)및 준수 & 로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="8d74e-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="8d74e-105">감사 **로그**  >  [**검색 검색을 선택합니다.**](https://go.microsoft.com/fwlink/?linkid=2103759)</span><span class="sxs-lookup"><span data-stu-id="8d74e-105">Select **Search** > [**Audit log search**](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>
    > [!NOTE]
    > <span data-ttu-id="8d74e-106">기능을 켜야 하다는 알림이 표시면 진행하여 지금 켜야 합니다.</span><span class="sxs-lookup"><span data-stu-id="8d74e-106">If you see a notice that you need to turn on the feature, go ahead and turn it on now.</span></span> <span data-ttu-id="8d74e-107">이 기능이 켜져 있지 않은 경우 검색 결과에서 이전 날짜의 데이터를 끌어오지 못합니다.</span><span class="sxs-lookup"><span data-stu-id="8d74e-107">If the feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="8d74e-108">활동을 **선택한** 다음 **Exchange 사서함 활동을 찾습니다.**</span><span class="sxs-lookup"><span data-stu-id="8d74e-108">Select **Activities**, and then find **Exchange mailbox activities**.</span></span> <span data-ttu-id="8d74e-109">**지우기 항목 폴더에서** 지우기 메시지 및 **지우기** 항목 폴더로 메시지 이동 옵션을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="8d74e-109">Select the **Deleted messages from Deleted Items** folder and **Moved messages to Deleted Items** folder options.</span></span> <span data-ttu-id="8d74e-110">완료되면 창 외부를 클릭하여 활동 창을 **최소화합니다.**</span><span class="sxs-lookup"><span data-stu-id="8d74e-110">When you're done, click outside of the pane to minimize the **Activities** pane.</span></span>
1. <span data-ttu-id="8d74e-111">날짜 범위를 지정하고 사용자  상자에서 조사할 사용자의 사용자 이름을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="8d74e-111">Specify the date range, and then in the **Users** box, select the username for the user you want to investigate.</span></span> <span data-ttu-id="8d74e-112">한에 두 개 이상의 사용자를 선택할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8d74e-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="8d74e-113">검색 **을 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="8d74e-113">Select **Search**.</span></span> <span data-ttu-id="8d74e-114">활동은 결과 아래에 **표시됩니다.**</span><span class="sxs-lookup"><span data-stu-id="8d74e-114">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="8d74e-115">세부 정보를 확인하려면 활동을 선택한 다음 추가 정보 **를 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="8d74e-115">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="8d74e-116">제목 줄 및 삭제된 항목의 위치와 같은 삭제된 항목에 대한 추가 정보가 **AffectedItems** 필드에 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="8d74e-116">Additional information about the deleted item, such as the subject line and the location of the item when it was deleted, is displayed in the **AffectedItems** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="8d74e-117">감사 로그 기능을 사용하여 삭제된 항목은 복원할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="8d74e-117">You can't restore deleted items using the audit log feature.</span></span> <span data-ttu-id="8d74e-118">삭제된 항목을 복원하려면 에서 삭제된 항목 또는 전자 메일 [복구를 Outlook Web App.](https://go.microsoft.com/fwlink/?linkid=2103759)</span><span class="sxs-lookup"><span data-stu-id="8d74e-118">To restore deleted items, see [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>

<span data-ttu-id="8d74e-119">자세한 내용은 [Office 365](https://go.microsoft.com/fwlink/?linkid=2103944)감사 로그 검색을 참조하여 일반적인 시나리오 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="8d74e-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
