---
title: 프로필 동기화
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: eee1080a95955332e205db3852381e39aaf5ae0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801775"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="46496-102">내 프로필 변경 내용이 SharePoint 사용자 프로필 응용 프로그램에 동기화 되는 경우</span><span class="sxs-lookup"><span data-stu-id="46496-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="46496-103">SharePoint Online에서는 Active Directory 가져오기 타이머 작업 (AD 가져오기)을 사용 하 여 사용자 및 그룹을 User Profile Application로 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="46496-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="46496-104">AD 가져오기에서는 SharePoint Online 디렉터리 저장소의 변경 내용을 사용자 프로필 응용 프로그램에 동기화 합니다.</span><span class="sxs-lookup"><span data-stu-id="46496-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="46496-105">이러한 변경 내용은 일괄적으로 처리 됩니다.</span><span class="sxs-lookup"><span data-stu-id="46496-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="46496-106">타이머 작업은 변경 내용이 동기화 될 때까지 실행 됩니다.</span><span class="sxs-lookup"><span data-stu-id="46496-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="46496-107">작업을 실행 하는 데 소요 되는 시간은 프로세스에 대 한 변경 수에 따라 달라 집니다.</span><span class="sxs-lookup"><span data-stu-id="46496-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="46496-108">많은 수의 변경 내용이 더 오래 걸립니다.</span><span class="sxs-lookup"><span data-stu-id="46496-108">A large number of changes takes longer.</span></span> <span data-ttu-id="46496-109">SLA (서비스 수준 계약)에는 SharePoint Online 디렉터리의 사용자 변경 내용이 24 시간 내에 사용자 프로필 응용 프로그램에 반영 된다는 내용이 나와 있습니다.</span><span class="sxs-lookup"><span data-stu-id="46496-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="46496-110">SharePoint Online의 사용자 프로필 동기화에 대 한 자세한 정보</span><span class="sxs-lookup"><span data-stu-id="46496-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

