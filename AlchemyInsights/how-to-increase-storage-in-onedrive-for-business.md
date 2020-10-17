---
title: 비즈니스용 OneDrive에서 저장소를 늘리는 방법
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ceaa6256-a9d9-4fef-a274-d7219365e07f
ms.openlocfilehash: 676b17d47ee5071ed45e8d6022eaa82b51fc4d51
ms.sourcegitcommit: ad2d185aa9e08c27c4a1c4803b679cc4e6305703
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/16/2020
ms.locfileid: "48489027"
---
# <a name="how-to-increase-storage-in-onedrive-for-business"></a><span data-ttu-id="716f5-102">비즈니스용 OneDrive에서 저장소를 늘리는 방법</span><span class="sxs-lookup"><span data-stu-id="716f5-102">How to increase storage in OneDrive for Business</span></span>

<span data-ttu-id="716f5-103">신규 및 기존 OneDrive 사용자에 대 한 기본 저장소를 변경 하려면:</span><span class="sxs-lookup"><span data-stu-id="716f5-103">To change the default storage for new and existing OneDrive users:</span></span>
  
- <span data-ttu-id="716f5-104">[OneDrive 관리 센터의 저장소 페이지로](https://admin.onedrive.com/?v=StorageSettings)이동 하 여 새 크기 (GB)를 입력 한 다음 **저장**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="716f5-104">Go to the [Storage page of the OneDrive admin center](https://admin.onedrive.com/?v=StorageSettings), enter a new amount in GB, then select **Save**.</span></span>

<span data-ttu-id="716f5-105">이 저장 공간 설정은 특정 저장 용량 제한을 설정 하지 않은 모든 사용자에 게 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="716f5-105">This storage space setting applies to all users for whom you haven't set specific storage limits.</span></span> <span data-ttu-id="716f5-106">특정 사용자에 대 한 저장소 공간을 변경 하려면 Microsoft PowerShell을 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="716f5-106">To change the storage space for specific users, use Microsoft PowerShell.</span></span> <span data-ttu-id="716f5-107">이 작업을 수행 하는 방법에 대 한 자세한 내용은 [PowerShell을 사용 하 여 사용자의 OneDrive 저장소 공간 변경을](https://docs.microsoft.com/onedrive/change-user-storage)참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="716f5-107">For info on how to do this, see [Change your users' OneDrive storage space using PowerShell](https://docs.microsoft.com/onedrive/change-user-storage).</span></span>

<span data-ttu-id="716f5-108">**참고**: 무제한 저장소를 포함 하는 계획이 없는 것 처럼 보입니다.</span><span class="sxs-lookup"><span data-stu-id="716f5-108">**NOTE**: It looks like you don't have a plan that includes unlimited storage.</span></span> <span data-ttu-id="716f5-109">각 요금제와 함께 제공 되는 저장소에 대 한 자세한 내용은 [비즈니스용 OneDrive 서비스 설명을](https://docs.microsoft.com/office365/servicedescriptions/onedrive-for-business-service-description)참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="716f5-109">For info about the storage that comes with each plan, see [OneDrive for Business service description](https://docs.microsoft.com/office365/servicedescriptions/onedrive-for-business-service-description).</span></span>
  
<span data-ttu-id="716f5-110">비즈니스용 OneDrive에서 저장소를 높이려면 **비즈니스용 Onedrive 계획 2** 또는 **Office 365 E3**을 포함 하는 구독을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="716f5-110">To increase your storage in OneDrive for Business, choose a subscription that includes either **OneDrive for Business Plan 2** or **Office 365 E3**.</span></span>
  
<span data-ttu-id="716f5-111">요금제를 변경 하려면 관리 센터에서 제품 **대금 청구** 페이지로 이동 하 여 \> [Your products](https://go.microsoft.com/fwlink/p/?linkid=842054) 변경할 구독을 선택한 다음, **조직에 권장 되는 업그레이드 보기**를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="716f5-111">To change plans, in the admin center, go to the **Billing** \> [Your products](https://go.microsoft.com/fwlink/p/?linkid=842054) page, select the subscription to change, then choose **View upgrades recommended for your org**.</span></span>
  
<span data-ttu-id="716f5-112">계획 및 비즈니스용 OneDrive 저장소를 변경 하는 방법에 대 한 자세한 내용은 [다른 요금제로 업그레이드](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan) 및 [비즈니스용 onedrive 서비스 설명을](https://docs.microsoft.com/office365/servicedescriptions/onedrive-for-business-service-description)참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="716f5-112">For more information on changing plans and OneDrive for Business storage, see [Upgrade to a different plan](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan) and the [OneDrive for Business Service Description](https://docs.microsoft.com/office365/servicedescriptions/onedrive-for-business-service-description).</span></span>