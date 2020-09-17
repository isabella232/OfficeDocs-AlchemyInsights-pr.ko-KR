---
title: SharePoint Online 제한
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 21d0f8d0118d92562b425921742513157563b5fb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773853"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="39a20-102">SharePoint Online 제한</span><span class="sxs-lookup"><span data-stu-id="39a20-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="39a20-103">**중요**: 이 시기에는 SharePoint Online 및 OneDrive 서비스를 항상 사용할 수 있도록 하는 단계를 진행하고 있습니다. 자세한 내용은 [SharePoint Online 임시 기능 조정](https://aka.ms/ODSPAdjustments)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="39a20-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="39a20-104">**503 서버 사용 중 오류**</span><span class="sxs-lookup"><span data-stu-id="39a20-104">**503 server is busy error**</span></span>

<span data-ttu-id="39a20-105">SharePoint 또는 OneDrive 사이트로 이동 하려고 하면 사용자에 게 503 서버가 통화 중 이라는 오류가 표시 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="39a20-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="39a20-106">이 오류는 SharePoint 서비스 내의 제한으로 인해 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="39a20-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="39a20-107">SharePoint Online은 제한된 기능을 사용하여 SharePoint Online 서비스의 최상의 성능과 안정성을 유지합니다.</span><span class="sxs-lookup"><span data-stu-id="39a20-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="39a20-108">제한 기능은 사용자 작업 수 또는 동시 호출 수(스크립트 또는 코드에 의한)를 제한하여 리소스가 과도하게 사용되지 않도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="39a20-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="39a20-109">제한에 대 한 자세한 내용은 [SharePoint Online에서 제한 또는 차단 되지 않도록](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)합니다 .를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="39a20-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="39a20-110">이 오류가 제한과 관련이 없는 것으로 생각 되는 경우 [메시지 센터로](https://portal.office.com/adminportal/home#/MessageCenter)이동 하 여 테 넌 트에서 활성 유지 관리가 진행 되 고 있는지 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="39a20-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="39a20-111">마지막으로 [서비스 상태](https://portal.office.com/adminportal/home#/servicehealth) 페이지를 방문 하 여 발생할 수 있는 권고/인시던트가 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="39a20-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

