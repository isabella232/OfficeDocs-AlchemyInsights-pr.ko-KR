---
title: 비즈니스용 OneDrive에서 저장소를 늘리는 방법
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ceaa6256-a9d9-4fef-a274-d7219365e07f
ms.openlocfilehash: 53eabf6c87dead3b7309c7da1f8a590940127169
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780101"
---
# <a name="how-to-increase-storage-in-onedrive-for-business"></a><span data-ttu-id="45eec-102">비즈니스용 OneDrive에서 저장소를 늘리는 방법</span><span class="sxs-lookup"><span data-stu-id="45eec-102">How to increase storage in OneDrive for Business</span></span>

<span data-ttu-id="45eec-103">신규 및 기존 OneDrive 사용자에 대 한 기본 저장소를 변경 하려면:</span><span class="sxs-lookup"><span data-stu-id="45eec-103">To change the default storage for new and existing OneDrive users:</span></span>
  
- <span data-ttu-id="45eec-104">[OneDrive 관리 센터의 저장소 페이지로](https://admin.onedrive.com/?v=StorageSettings)이동한 다음 새 금액 (GB)을 입력 합니다.</span><span class="sxs-lookup"><span data-stu-id="45eec-104">Go to the [Storage page of the OneDrive admin center](https://admin.onedrive.com/?v=StorageSettings), and then enter a new amount in GB.</span></span>

<span data-ttu-id="45eec-105">이 저장 공간 설정은 특정 저장 용량 제한을 설정 하지 않은 모든 사용자에 게 적용 됩니다.</span><span class="sxs-lookup"><span data-stu-id="45eec-105">This storage space setting applies to all users for whom you haven't set specific storage limits.</span></span> <span data-ttu-id="45eec-106">특정 사용자에 대 한 저장소 공간을 변경 하려면 Microsoft PowerShell을 사용 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="45eec-106">To change the storage space for specific users, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="45eec-107">이 작업을 수행 하는 방법에 대 한 자세한 내용은 [PowerShell을 사용 하 여 사용자의 OneDrive 저장소 공간 변경을](https://go.microsoft.com/fwlink/?linkid=866402)참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="45eec-107">For info on how to do this, see [Change your users' OneDrive storage space using PowerShell](https://go.microsoft.com/fwlink/?linkid=866402).</span></span>

<span data-ttu-id="45eec-108">**참고**: 무제한 저장소를 포함 하는 계획이 없는 것 처럼 보입니다.</span><span class="sxs-lookup"><span data-stu-id="45eec-108">**NOTE**: It looks like you don't have a plan that includes unlimited storage.</span></span> <span data-ttu-id="45eec-109">각 요금제와 함께 제공 되는 저장소에 대 한 자세한 내용은 [비즈니스용 OneDrive 서비스 설명을](https://go.microsoft.com/fwlink/p/?LinkID=826071)참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="45eec-109">For info about the storage that comes with each plan, see [OneDrive for Business service description](https://go.microsoft.com/fwlink/p/?LinkID=826071).</span></span>
  
<span data-ttu-id="45eec-110">비즈니스용 OneDrive에서 저장소를 향상 시키려면 **비즈니스용 Onedrive 계획 2** 또는 **Office 365 Enterprise**e 3이 포함 된 구독을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="45eec-110">To increase your storage in OneDrive for Business, choose a subscription that includes either **OneDrive for Business Plan 2** or **Office 365 Enterprise E3**.</span></span> 
  
<span data-ttu-id="45eec-111">요금제를 변경 하려면 Microsoft 365 관리 센터에서 제품 **대금 청구** 페이지로 이동 하 여 \> **[Your products](https://go.microsoft.com/fwlink/p/?linkid=842054)** 변경할 구독을 선택한 다음 **업그레이드** 탭을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="45eec-111">To change plans, in the Microsoft 365 admin center, go to the **Billing** \> **[Your products](https://go.microsoft.com/fwlink/p/?linkid=842054)** page, select the subscription to change, and then choose the **Upgrade** tab.</span></span>
  
<span data-ttu-id="45eec-112">요금제 및 비즈니스용 OneDrive 저장소를 전환 하는 방법에 대 한 자세한 내용은 [다른 Microsoft 365 for business 요금제](https://go.microsoft.com/fwlink/?LinkId=2031117) 및 [비즈니스용 onedrive 서비스 설명을](https://go.microsoft.com/fwlink/p/?LinkId-2031122)참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="45eec-112">For more information on switching plans and OneDrive for Business storage, see [Switch to a different Microsoft 365 for business plan](https://go.microsoft.com/fwlink/?LinkId=2031117) and the [OneDrive for Business Service Description](https://go.microsoft.com/fwlink/p/?LinkId-2031122).</span></span>