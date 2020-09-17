---
title: 차트에서 다양한 수의 레코드를 표로 표시
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: e499a439e7cf7e9ecbb6566f9f089f3b7b82f48e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47793764"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a><span data-ttu-id="97ad1-102">차트에서 다양한 수의 레코드를 표로 표시</span><span class="sxs-lookup"><span data-stu-id="97ad1-102">Chart shows different number of records in grid</span></span>

<span data-ttu-id="97ad1-103">**증상**</span><span class="sxs-lookup"><span data-stu-id="97ad1-103">**Symptom**</span></span>

<span data-ttu-id="97ad1-104">대시보드 페이지의 차트에서 차트 "…"를 클릭하고 "레코드 보기"를 클릭하면 표 페이지로 이동하여 모든 레코드를 볼 수 있습니다. 가끔 레코드 수가 변경되는 경우도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="97ad1-104">For chart on dashboard page, when you click on chart "…" and click "View records", you navigate to grid page to see all the records.Sometimes, the number of records changes.</span></span>

<span data-ttu-id="97ad1-105">**원인**</span><span class="sxs-lookup"><span data-stu-id="97ad1-105">**Cause**</span></span>

<span data-ttu-id="97ad1-106">이는 원본 대시보드 페이지의 차트와 표 홈 페이지의 차트 간에 차이가 있기 때문입니다.</span><span class="sxs-lookup"><span data-stu-id="97ad1-106">This is due to the difference of views between the chart on the original dashboard page and the chart on the grid home page.</span></span>  

<span data-ttu-id="97ad1-107">**솔루션**</span><span class="sxs-lookup"><span data-stu-id="97ad1-107">**Solution**</span></span>

1. <span data-ttu-id="97ad1-108">원본 페이지의 보기와 표의 보기가 서로 다른지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="97ad1-108">Check the view from the original page and the view in the grid to see if they are different.</span></span>
2. <span data-ttu-id="97ad1-109">원본 페이지의 보기에 맞게 표의 보기를 변경합니다.</span><span class="sxs-lookup"><span data-stu-id="97ad1-109">Change the view in grid to match the view in the original page.</span></span>
3. <span data-ttu-id="97ad1-110">올바른 보기를 찾을 수 없는 경우 일반적으로 이는 앱 디자이너에서 보기를 사용하도록 설정되어 있지 않음을 나타냅니다.</span><span class="sxs-lookup"><span data-stu-id="97ad1-110">If the correct view cannot be found, usually it means the view is not enabled in app designer.</span></span>
4. <span data-ttu-id="97ad1-111">특정 앱의 앱 디자이너로 이동하여 엔터티와 해당 보기를 선택한 후 사용하도록 설정하고, 저장하고, 게시하고, 닫으려는 보기를 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="97ad1-111">Go to app designer of the specific app, choose the entity and its views, check the view you want to enable, save, publish and close.</span></span>
5. <span data-ttu-id="97ad1-112">페이지를 새로 고칩니다.</span><span class="sxs-lookup"><span data-stu-id="97ad1-112">Refresh the page.</span></span>