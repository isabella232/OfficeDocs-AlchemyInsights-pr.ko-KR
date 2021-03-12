---
title: 액세스 거부 메시지 문제 해결
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704900"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="28f13-102">액세스 거부 메시지 문제 해결</span><span class="sxs-lookup"><span data-stu-id="28f13-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="28f13-103">누군가 SharePoint의 공유 폴더에 대한 "액세스 거부" 메시지가 표시되면 사이트 모음 관리자가 "제한된 액세스 사용자 권한 잠금 모드"를 사용하도록 설정한 것일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="28f13-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="28f13-104">이 기능을 끄는 경우:</span><span class="sxs-lookup"><span data-stu-id="28f13-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="28f13-105">사이트로 이동하여 설정 아이콘을 클릭한 다음 사이트 **설정을 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="28f13-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="28f13-106">**사이트 모음 관리** 에서 **사이트 모음 기능** 을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="28f13-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="28f13-107">제한된 액세스 사용자 권한 잠금 **모드 옆의** **비활성화를 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="28f13-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="28f13-108">사이트가 게시 사이트인 경우 공유 폴더에 대한 액세스 거부 메시지도 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="28f13-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="28f13-109">자세한 내용은 공유 폴더에 액세스할 때 [액세스 거부를 참조하세요.](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb)</span><span class="sxs-lookup"><span data-stu-id="28f13-109">For info, see [Access Denied when accessing a shared folder](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span></span>
  
<span data-ttu-id="28f13-110">액세스 요청을 보려고 할 때 "액세스 거부" 메시지가 표시될 경우 해당 사용자를 사이트 모음 관리자 또는 사이트의 Owners 그룹 구성원으로 추가해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="28f13-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="28f13-111">자세한 내용은 액세스 요청 목록에 대한 [액세스 거부를 참조하세요.](https://go.microsoft.com/fwlink/?linkid=2004220)</span><span class="sxs-lookup"><span data-stu-id="28f13-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="28f13-112">사용자가 Active Directory에서 제거된 후 다시 추가된 후 "액세스 거부" 메시지가 표시되면 사용자 계정이 [Microsoft 365와](https://go.microsoft.com/fwlink/?linkid=2004318)동기화될 때 액세스 거부를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="28f13-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

