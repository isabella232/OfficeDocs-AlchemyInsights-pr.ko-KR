---
title: SharePoint 또는 OneDrive를 사용 하려고 할 때 유지 관리 메시지에 대 한 읽기 전용
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670838"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="199cd-102">SharePoint 또는 OneDrive를 사용 하려고 할 때 유지 관리 메시지에 대 한 읽기 전용</span><span class="sxs-lookup"><span data-stu-id="199cd-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="199cd-103">사용자는 다음 시나리오 중 하나에 대해 SharePoint 또는 OneDrive를 사용 하려고 할 때 **유지 관리 메시지에 대 한 읽기 전용** 을 받을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="199cd-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="199cd-104">계획 된 또는 활성 유지 관리 활동</span><span class="sxs-lookup"><span data-stu-id="199cd-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="199cd-105">[메시지 센터](https://portal.office.com/adminportal/home#/messagecenter)를 탐색 하 여 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="199cd-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="199cd-106">발생할 수 있는 높은 우선 순위의 활성 서비스 인시던트</span><span class="sxs-lookup"><span data-stu-id="199cd-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="199cd-107">[서비스 상태](https://portal.office.com/adminportal/home#/servicehealth)를 탐색 하 여 모든 권고/인시던트를 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="199cd-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="199cd-108">서버에 대 한 예기치 않은 이벤트 (30 분 미만)로 인해 발생할 수 있는 사소한 자동 복구 복구 시나리오입니다.</span><span class="sxs-lookup"><span data-stu-id="199cd-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="199cd-109">이러한 사소한 복구를 위한 메시지 센터 또는 서비스 상태 게시물은 제공 되지 않지만 곧 정상적으로 백업 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="199cd-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="199cd-110">위의 세 가지 시나리오 중 하나에 문제가 발생 하 여 서비스를 복원 했지만 사용자 브라우저 캐시가 지워지지 않은 경우도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="199cd-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="199cd-111">사이트를 탐색 하기 전에 브라우저 캐시를 지워야 합니다.</span><span class="sxs-lookup"><span data-stu-id="199cd-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="199cd-112">Microsoft Edge 브라우저에서 **설정을**선택한 다음 **개인 정보 및 보안**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="199cd-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="199cd-113">**검색 지우기**에서 **지우려는 작업**선택을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="199cd-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="199cd-114">**쿠키 및 저장 된 웹 사이트 데이터**를 선택 하 고 **지우기를**선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="199cd-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="199cd-115">Mozilla Firefox 또는 Google Chrome과 같은 다른 브라우저를 사용 하는 경우에는 이러한 단계가 다를 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="199cd-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="199cd-116">또 다른 옵션으로는 SharePoint 사이트 또는 OneDrive를 새 InPrivate 창에서 열 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="199cd-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>