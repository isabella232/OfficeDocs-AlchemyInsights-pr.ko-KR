---
title: 워크플로가 시작되지 않습니다.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403749"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="be873-102">워크플로가 시작되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="be873-102">Workflow is not starting</span></span>

- <span data-ttu-id="be873-103">SharePoint 2010 및 SharePoint 2013 워크플로가 시작되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="be873-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="be873-104">워크플로가 시작되지 않는 경우 워크플로 진행률에 따라 사용자에게 일시적인 지연이 생략될 수 있는 임시 서비스 문제가 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="be873-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="be873-105">서비스 상태 [대시보드를](https://admin.microsoft.com/AdminPortal/Home/servicehealth) 확인하여 조직에 영향을 미치는지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="be873-105">Check the [Service Health Dashboard](https://admin.microsoft.com/AdminPortal/Home/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="be873-106">이 문제가 처음 확인된 후 24시간 이상이 지난 경우 지원 티켓을 기록하세요.</span><span class="sxs-lookup"><span data-stu-id="be873-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="be873-107">대부분의 경우 당사는 이미 해결 방법에 대한 작업을 하고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="be873-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="be873-108">솔루션을 완료하는 데 최소 24시간을 기다렸다가 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="be873-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="be873-109">시작 시 SharePoint 2010 워크플로가 지연됩니다.</span><span class="sxs-lookup"><span data-stu-id="be873-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="be873-110">워크플로가 대규모 일괄 처리에서 트리거되는 경우 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="be873-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="be873-111">예를 들어 한에 여러 항목이 추가된 경우입니다.</span><span class="sxs-lookup"><span data-stu-id="be873-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="be873-112">워크플로는 실시간으로 실행하도록 설계되지 않은 것이기 때문에 지연은 디자인된 동작입니다.</span><span class="sxs-lookup"><span data-stu-id="be873-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="be873-113">워크플로가 XMOL(Extensible Object Markup Language)이 복잡하면 컴파일 속도가 느려질 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="be873-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="be873-114">이 [문서를 확인](https://support.microsoft.com//kb/3043697) 합니다.</span><span class="sxs-lookup"><span data-stu-id="be873-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="be873-115">Microsoft SharePoint 2013 워크플로 플랫폼 유형을 사용하여 워크플로를 단순화하거나 다시 디자인해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="be873-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="be873-116">워크플로 기록이 커진 경우 항목을 제거하거나 새 기록 목록을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="be873-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="be873-117">추가 정보: [워크플로 기록 제거](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="be873-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="be873-118">관련 항목</span><span class="sxs-lookup"><span data-stu-id="be873-118">Related topics</span></span>
<span data-ttu-id="be873-119">SharePoint Online에서 Microsoft Flow를 사용해 보시겠습니까?</span><span class="sxs-lookup"><span data-stu-id="be873-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="be873-120">흐름 만들기</span><span class="sxs-lookup"><span data-stu-id="be873-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="be873-121">SharePoint 및 Flow</span><span class="sxs-lookup"><span data-stu-id="be873-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
