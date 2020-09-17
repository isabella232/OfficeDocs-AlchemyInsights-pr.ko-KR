---
title: 마이그레이션 중 사용 권한 문제
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: cbec51a7-5513-4848-a9ae-cdf993e000a8
ms.openlocfilehash: 39b36a85319ccd71278571f3a3cbbc7cf0b9f0fa
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798058"
---
# <a name="user-profile-and-photo-synchronization"></a><span data-ttu-id="54163-102">사용자 프로필 및 사진 동기화</span><span class="sxs-lookup"><span data-stu-id="54163-102">User Profile and Photo synchronization</span></span>

 <span data-ttu-id="54163-103">**프로필 사진 동기화** -사용자가 프로필 사진을 SharePoint와 동기화 하지 않는 것을 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="54163-103">**Profile Photo Synchronization** - Users may notice that their profile photo is not synchronizing to SharePoint.</span></span> <span data-ttu-id="54163-104">또는 사용자가 프로필 사진을 업데이트 하려고 했지만 사진이 여전히 이전 사진으로 표시 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="54163-104">Or, they may have tried to update their profile photo and the photo still appears as the old photo.</span></span> <span data-ttu-id="54163-105">프로필 사진이 예상 대로 표시 되도록 하려면 사용자가 사진 동기화를 시작 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="54163-105">To ensure the profile photo shows as expected, the user will need to initiate a photo sync.</span></span> 
  
<span data-ttu-id="54163-106">사진 동기화 프로세스에 대 한 자세한 내용은 [Microsoft 365에서 프로필 그림 동기화에 대 한 정보](https://go.microsoft.com/fwlink/?linkid=2022634) 를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="54163-106">For more information about the photo synchronization process, see [Information about profile picture synchronization in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span></span>
  
- <span data-ttu-id="54163-107">**프로필 동기화** -프로필 동기화를 완료 하는 데 필요한 시간은 AD 가져오기 작업에서 처리 해야 하는 변경 내용 (작업) 수에 따라 달라 집니다.</span><span class="sxs-lookup"><span data-stu-id="54163-107">**Profile Synchronization** - The time that's required to complete a profile synchronization depends on the number of changes (work) the AD Import Job has to process.</span></span> <span data-ttu-id="54163-108">변경 내용이 많은 경우에는 타이머 작업에 많은 작업을 수행 해야 하므로 변경 내용이 사용자 프로필 응용 프로그램에 반영 되는 데 시간이 오래 걸립니다.</span><span class="sxs-lookup"><span data-stu-id="54163-108">If there are many changes, the timer job has a lot of work to do, and it will take longer for the changes to be reflected in the User Profile Application.</span></span> <span data-ttu-id="54163-109">타이머 작업에 작업 양이 많지 않은 경우 변경 내용이 사용자 프로필 응용 프로그램에 훨씬 더 빠르게 반영 됩니다.</span><span class="sxs-lookup"><span data-stu-id="54163-109">If the timer job has a small volume of work to do, the changes will be reflected in the User Profile Application much faster.</span></span> 
  
<span data-ttu-id="54163-110">프로필 동기화 프로세스에 대 한 자세한 내용은 [SharePoint Online의 사용자 프로필 동기화 정보](https://go.microsoft.com/fwlink/?linkid=2022639) 를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="54163-110">For more information about the profile synchronization process, see [Information about user profile synchronization in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span></span>
    
- <span data-ttu-id="54163-111">**Office delve의 업데이트 프로필** -delve 사용자는 Microsoft 365 프로필을 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="54163-111">**Update Profile in Office Delve** - Delve users can manage their Microsoft 365 Profile.</span></span> <span data-ttu-id="54163-112">자세한 내용은 [Office Delve에서 프로필 보기 및 업데이트](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="54163-112">For more information, see [View and Update your profile in Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>
    

