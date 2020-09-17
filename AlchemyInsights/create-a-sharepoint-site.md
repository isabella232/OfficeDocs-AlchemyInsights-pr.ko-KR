---
title: SharePoint 사이트 만들기
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 5ebaa342ca9864bc31a9ef26eebcf42d96523871
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806945"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="7e313-102">SharePoint 사이트 만들기</span><span class="sxs-lookup"><span data-stu-id="7e313-102">Create a SharePoint site</span></span>

<span data-ttu-id="7e313-103">SharePoint 관리 센터의 [활성 사이트](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) 에서 사이트를 만들거나 관리 합니다.</span><span class="sxs-lookup"><span data-stu-id="7e313-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="7e313-104">자세한 내용은 [새 SharePoint 관리 센터에서 사이트 관리](https://docs.microsoft.com/sharepoint/manage-site-creation)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="7e313-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="7e313-105">정보</span><span class="sxs-lookup"><span data-stu-id="7e313-105">Tips:</span></span>

- <span data-ttu-id="7e313-106">기존 사이트와 동일한 URL을 사용 하 여 사이트를 만들 **수는 없습니다** .</span><span class="sxs-lookup"><span data-stu-id="7e313-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="7e313-107">사이트를 삭제 하 고 해당 URL을 다시 사용 하려는 [경우 삭제 된 사이트 아래에](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true)해당 사이트가 계속 남아 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7e313-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="7e313-108">URL을 다시 사용 하려면 사이트를 영구적으로 삭제 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="7e313-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="7e313-109">Powershell을 사용 하 여 사이트를 완전히 제거 하려면 [제거-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet 예제를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="7e313-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="7e313-110">일부 사용자가 사이트를 만들지 못할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7e313-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="7e313-111">[SharePoint Online에서 사이트 만들기 관리를 참조](https://docs.microsoft.com/sharepoint/manage-site-creation)하세요.</span><span class="sxs-lookup"><span data-stu-id="7e313-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="7e313-112">사이트가 예상 보다 오래 **생성** 되는 것 처럼 표시 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7e313-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="7e313-113">이 문제가 처음 발생 한 것으로 24 시간 이상 경과 된 경우 지원 티켓을 기록 하세요.</span><span class="sxs-lookup"><span data-stu-id="7e313-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="7e313-114">대부분의 경우 당사는 이미 해결 방법에 대한 작업을 하고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7e313-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="7e313-115">솔루션을 완료 하려면 최소한 24 시간 이상 기다려 주세요.</span><span class="sxs-lookup"><span data-stu-id="7e313-115">Please give us at least 24 hours to complete a solution.</span></span>
