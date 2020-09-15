---
title: 누락 된 워크플로를 활성화 하지 못함
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 604dc770c5c14ded6a8de1cec9e311b03b69f094
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667092"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="49963-102">누락 된 워크플로를 활성화 하지 못함</span><span class="sxs-lookup"><span data-stu-id="49963-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="49963-103">Microsoft SharePoint 사이트 모음에서는 목록 또는 라이브러리에 전역으로 다시 사용 가능한 워크플로 (예: "승인-SharePoint 2010")를 추가할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="49963-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="49963-104">이 문제를 해결 하려면 다음 단계를 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="49963-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="49963-105">SharePoint Designer 2013에서 사이트 모음의 루트 웹 사이트를 엽니다.</span><span class="sxs-lookup"><span data-stu-id="49963-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="49963-106">**사이트 개체**에서 **워크플로**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="49963-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="49963-107">**워크플로** 리본 메뉴의 **새로 만들기** 섹션에서 **다시 사용할**수 있는 워크플로를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="49963-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="49963-108">**다시 사용할 수 있는 워크플로 만들기** 양식에서 \* \* *Repair2010* \* \* 이름을 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="49963-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="49963-109">**플랫폼 유형**으로 **SharePoint 2010 워크플로**를 클릭 한 다음 **확인**을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="49963-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="49963-110">**워크플로** 리본 메뉴의 **저장** 섹션에서 **게시**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="49963-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="49963-111">**워크플로** 리본 메뉴의 **관리** 섹션에서 **전역으로 게시**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="49963-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="49963-112">확인 대화 상자가 나타나면 **확인**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="49963-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="49963-113">웹 브라우저에서 사이트 모음의 루트 웹 사이트를 찾은 다음 **사이트 설정** \> **사이트 모음 기능**에 액세스 합니다.</span><span class="sxs-lookup"><span data-stu-id="49963-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="49963-114">그런 다음 **워크플로** 기능을 설정/해제 합니다.</span><span class="sxs-lookup"><span data-stu-id="49963-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="49963-115">· 기능이  *활성화*  되 면 **비활성화를** 클릭 한 다음 **활성화**를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="49963-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="49963-116">· 기능이  *비활성화*  되어 있으면 **활성화**를 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="49963-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="49963-117">자세한 내용은 다음 [문서](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="49963-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

