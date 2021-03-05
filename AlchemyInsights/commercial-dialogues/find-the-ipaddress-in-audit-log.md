---
title: 감사 로그에서 IP 주소 찾기
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
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50465005"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="a690d-102">감사 로그에서 IP 주소 찾기</span><span class="sxs-lookup"><span data-stu-id="a690d-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="a690d-103">사용자 또는 관리자가 수행한 활동에 해당하는 IP 주소가 감사 로그에 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="a690d-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="a690d-104">클라이언트 정보도 기록됩니다.</span><span class="sxs-lookup"><span data-stu-id="a690d-104">The client information is also logged.</span></span> <span data-ttu-id="a690d-105">IP 주소를 식별하는 방법에는 다음이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a690d-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="a690d-106">[Office 365 보안](https://go.microsoft.com/fwlink/p/?linkid=2077143)및 준수 & 로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="a690d-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="a690d-107">감사 **로그**  >  **[검색 검색을 선택합니다.](https://go.microsoft.com/fwlink/?linkid=2103759)**</span><span class="sxs-lookup"><span data-stu-id="a690d-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="a690d-108">감사를 켜야 하는 알림이 표시된 경우 지금 진행하여 켜야 합니다.</span><span class="sxs-lookup"><span data-stu-id="a690d-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="a690d-109">이 기능을 사용하도록 설정하지 않은 경우 검색 결과에서 이전 날짜의 데이터를 끌 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="a690d-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="a690d-110">특정 활동에 관심이 있는 경우 활동 목록에서 해당 활동을 **선택합니다.** 그렇지 않으면 기본적으로 선택한 사용자에 대한 모든 활동이 반환됩니다.</span><span class="sxs-lookup"><span data-stu-id="a690d-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="a690d-111">특정 활동은 활동 메뉴에서 선택하지 못하게 될 **수** 있습니다. 그러나 모든 활동에 대한 결과  표시를 선택한 경우(기본 설정) 해당 감사 항목이 반환됩니다.</span><span class="sxs-lookup"><span data-stu-id="a690d-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="a690d-112">날짜 범위를 지정하고 사용자 **필드에서** 조사할 사용자의 사용자 이름을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="a690d-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="a690d-113">검색 **을 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="a690d-113">Select **Search**.</span></span> <span data-ttu-id="a690d-114">활동은 결과 아래에 **표시됩니다.**</span><span class="sxs-lookup"><span data-stu-id="a690d-114">The activities appear under **Results**.</span></span> <span data-ttu-id="a690d-115">각 활동에 대한 IP 주소를 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a690d-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="a690d-116">세부 정보를 확인하려면 활동을 선택한 다음 추가 정보 **를 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="a690d-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="a690d-117">자세한 내용은 [Office 365](https://go.microsoft.com/fwlink/?linkid=2103944)감사 로그 검색을 참조하여 일반적인 시나리오 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="a690d-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>