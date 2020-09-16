---
title: 성능 문제-SharePoint 또는 OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771907"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="31007-102">여러 사용자가 SharePoint 또는 OneDrive에 느리거나, 액세스 하지 않거나, 사용할 수 없음</span><span class="sxs-lookup"><span data-stu-id="31007-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="31007-103">SharePoint 또는 OneDrive는 다음과 같은 몇 가지 이유로 인해 느리거나, 액세스 불가능 하거나, 사용할 수 없거나 서비스를 사용할 수 없거나 503 오류가 표시 될 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="31007-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="31007-104">SharePoint 또는 OneDrive 사이트가 여러 사용자에 대해 느리거나 지연 되는 경우 사용자가 SharePoint 사이트 또는 OneDrive 콘텐츠에 액세스할 때 일시적으로 지연 되거나 탐색 오류가 발생 하는 일시적인 서비스 문제가 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="31007-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="31007-105">조직에 영향을 미치는지 확인하려면 [서비스 상태 대시보드](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)를 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="31007-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="31007-106">SharePoint 또는 OneDrive 사이트로 이동 하려고 하면 사용자에 게 *503 서버가 통화 중* 이라는 오류가 표시 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="31007-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="31007-107">이 오류는 SharePoint 서비스 내의 제한으로 인해 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="31007-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="31007-108">SharePoint Online은 제한된 기능을 사용하여 SharePoint Online 서비스의 최상의 성능과 안정성을 유지합니다.</span><span class="sxs-lookup"><span data-stu-id="31007-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="31007-109">제한 기능은 사용자 작업 수 또는 동시 호출 수(스크립트 또는 코드에 의한)를 제한하여 리소스가 과도하게 사용되지 않도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="31007-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="31007-110">제한에 대 한 자세한 내용은 [SharePoint Online에서 제한 또는 차단 되지 않도록](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)합니다 .를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="31007-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="31007-111">**클래식** 또는 **최신** SharePoint 사이트나 페이지로 인 한 성능이 저하 되는 경우 [페이지 진단 도구](https://aka.ms/perftool) 를 활용 하 여 페이지를 분석 합니다.</span><span class="sxs-lookup"><span data-stu-id="31007-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="31007-112">여전히 일반적인 성능 저하가 발생 하는 경우이 문서 아래쪽의 리소스를 검토 하세요. [SharePoint Online의 성능 조정 소개](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="31007-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  