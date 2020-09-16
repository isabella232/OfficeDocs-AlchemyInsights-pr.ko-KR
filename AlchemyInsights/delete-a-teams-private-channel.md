---
title: Teams 개인 채널 삭제
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
- "3781"
- "9001223"
ms.openlocfilehash: 56021a335c64810700913cf08519b95f24a7a17d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730921"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="85ad7-102">Teams 개인 채널 삭제</span><span class="sxs-lookup"><span data-stu-id="85ad7-102">Delete a Teams private channel</span></span>

<span data-ttu-id="85ad7-103">Microsoft는 기본 SharePoint 사이트에 SharePoint 보존 정책을 사용하는 경우 Teams 개인 채널을 삭제하는 데 문제를 알고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85ad7-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="85ad7-104">Microsoft는 문제 해결을 위해 노력하고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85ad7-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="85ad7-105">그 동안에는 다음 해결 방법을 사용하여 개인 채널을 삭제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85ad7-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="85ad7-106">**Sharepoint 보존 정책에서 팀/사이트 모음을 제외시킵니다.**</span><span class="sxs-lookup"><span data-stu-id="85ad7-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="85ad7-107">Office 365 관리 포털로 이동하고 왼쪽 탐색 창에서 **모두 표시**를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="85ad7-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="85ad7-108">**관리 센터**에서 **보안 및 규정 준수** > **데이터 손실 방지** > **정책**으로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="85ad7-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="85ad7-109">Sharepoint 사이트에 적용되는 모든 정책을 식별하고, 개인 채널을 포함하는 팀의 Sharepoint 사이트가 보존 정책에 포함되지 않도록 정책을 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="85ad7-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="85ad7-110">정책을 저장합니다.</span><span class="sxs-lookup"><span data-stu-id="85ad7-110">Save the policy.</span></span>
    <span data-ttu-id="85ad7-111">정책 설정이 적용되는 데 최대 24시간이 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85ad7-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="85ad7-112">사이트를 제외한 후에 개인 채널을 삭제할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="85ad7-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="85ad7-113">Android 장치에서 Microsoft Teams를 사용하여 개인 채널을 삭제***할 수 있습니다***.</span><span class="sxs-lookup"><span data-stu-id="85ad7-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="85ad7-114">관련 SharePoint에 대한 정보를 보려면 [SharePoint Online 또는 비즈니스용 OneDrive에서 항목을 삭제할 수 없음](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="85ad7-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>