---
title: 삭제된 사이트 복원
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 570284765f32212b4ef2062db5b70f427b28c121
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47692049"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="13615-102">삭제된 사이트 복원</span><span class="sxs-lookup"><span data-stu-id="13615-102">Restore a deleted site</span></span>

<span data-ttu-id="13615-103">관리자가 SharePoint 사이트를 삭제 하면 사이트가 영구적으로 삭제 되기 전까지 93 일 전에 보관 되는 사이트 모음 휴지통에 저장 됩니다.</span><span class="sxs-lookup"><span data-stu-id="13615-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="13615-104">사이트를 복원 하려면</span><span class="sxs-lookup"><span data-stu-id="13615-104">To restore the site:</span></span>
  
1. <span data-ttu-id="13615-105">새 SharePoint 관리 센터에서 리본 메뉴의 **휴지통** 을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="13615-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="13615-106">복원 하려는 사이트 모음 옆에 있는 확인란을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="13615-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="13615-107">**지운 편지함 복원을**클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="13615-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="13615-108">삭제 된 통신 사이트를 복원 하려면 새 SharePoint 관리 센터를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="13615-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="13615-109">그렇지 않으면 Microsoft PowerShell을 사용 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="13615-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="13615-110">Microsoft 365 그룹에 속하는 사이트를 복원 하려면 Exchange 관리 센터에서 그룹을 복원 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="13615-110">To restore a site that belongs to a Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="13615-111">그룹을 삭제 한 후 30 일 동안 복원할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="13615-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

