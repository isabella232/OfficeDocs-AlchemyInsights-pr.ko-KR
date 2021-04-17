---
title: SharePoint 루트 사이트 삭제
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
- "9003017"
- "5727"
ms.openlocfilehash: 849c5c58ab4688130d71baffac8fe39eddf92f18
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815477"
---
# <a name="delete-the-sharepoint-root-site"></a><span data-ttu-id="3754c-102">SharePoint 루트 사이트 삭제</span><span class="sxs-lookup"><span data-stu-id="3754c-102">Delete the SharePoint root site</span></span>

<span data-ttu-id="3754c-103">SharePoint 루트 사이트 삭제는 **지원되지 않습니다**.</span><span class="sxs-lookup"><span data-stu-id="3754c-103">Deleting the SharePoint root site is  **not supported.**</span></span>

1.  <span data-ttu-id="3754c-104">루트 사이트가 이미 삭제된 경우 사이트에 액세스하려고 할 때 404 File Not Found(파일 찾을 수 없음) 오류가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="3754c-104">If the root site has already been deleted, users will experience a  404 File Not Found  error when trying to access the site.</span></span>
2.  <span data-ttu-id="3754c-105">문제를 해결하려면 새 SharePoint 관리 센터에서 [삭제된 사이트](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) 페이지로 이동하여 루트 사이트를 선택하고 복원을 클릭하여 사이트를 복원합니다.</span><span class="sxs-lookup"><span data-stu-id="3754c-105">To resolve, restore the site  from the new SharePoint admin center by going to the  [Deleted sites](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true)  page, select the root site and click  Restore.</span></span>
3.  <span data-ttu-id="3754c-106">루트 사이트가 복원되면 루트 사이트를 삭제하는 대신 새 SharePoint 관리 센터에서 [사이트 바꾸기](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site)를 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="3754c-106">Instead of deleting the root site, use [replace site](https://docs.microsoft.com/sharepoint/modern-root-site#replace-your-root-site)  from the new SharePoint Admin Center once the root site is restored.</span></span>

<span data-ttu-id="3754c-107">자세한 내용은 [루트 사이트 현대화하기](https://docs.microsoft.com/sharepoint/modern-root-site)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="3754c-107">For more info, see [Modernize your root site](https://docs.microsoft.com/sharepoint/modern-root-site)</span></span>