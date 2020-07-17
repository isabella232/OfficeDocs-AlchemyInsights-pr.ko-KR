---
title: Yammer 라이선스 문제
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45146809"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="84238-102">Yammer 라이선스 문제</span><span class="sxs-lookup"><span data-stu-id="84238-102">Yammer licensing issues</span></span>

<span data-ttu-id="84238-103">Yammer Enterprise 서비스를 사용하려는 모든 사용자는 라이선스를 보유하고 있어야 하지만 기본적으로 Yammer 서비스에 액세스 하는데 라이선스가 필요하지는 않습니다.</span><span class="sxs-lookup"><span data-stu-id="84238-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="84238-104">관리자가 Yammer 라이선스가 없는 Microsoft 365 사용자를 차단하도록 설정하면 Yammer Enterprise 라이선스를 할당하지 않는 사용자는 Yammer 서비스에 액세스 할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="84238-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="84238-105">자세한 내용은 [Office 365에서 Yammer 사용자 라이선스 관리](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="84238-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="84238-106">라이선스가 사용자에게서 삭제되면 Yammer 타일은 더 이상 보이지 않고 다른 서비스는 기능을 숨기기 위해 라이선스 삭제를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="84238-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="84238-107">경우에 따라 기능을 계속 사용할 수 있지만 운영하기 위해서는 라이선스 할당이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="84238-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="84238-108">**라이선스가 업데이트 되지 않습니다**</span><span class="sxs-lookup"><span data-stu-id="84238-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="84238-109">가끔 사용자에게 라이선스가 할당 되었지만 Yammer에 액세스 하지 못할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="84238-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="84238-110">대량 라이선스가 할당 되는 경우 지연이 발생 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="84238-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="84238-111">시스템이 비동기적으로 실행되므로 Azure AD에서 라이선스가 변경되는 것과 동일한 순서로 Yammer 사용자 업데이트가 되지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="84238-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="84238-112">라이선스 동기화 문제를 지원에 보고하기 전에 24시간을 기다립니다.</span><span class="sxs-lookup"><span data-stu-id="84238-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="84238-113">**대량 라이선스 할당**</span><span class="sxs-lookup"><span data-stu-id="84238-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="84238-114">라이선스는 관리 센터 또는 PowerShell 스크립트를 통해 할당할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="84238-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="84238-115">자세한 내용은 [사용자에게 라이선스 할당](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) 및 [Office 365 PowerShell 사용자 계정으로 라이선스 할당](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="84238-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="84238-116">Microsoft 지원에서는 스크립트 만들기 지원을 제공하지 않지만 Yammer 라이선스 할당 관련 문서를 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="84238-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="84238-117">자세한 내용은 [Windows PowerShell을 사용하여 Yammer 라이선스 관리](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="84238-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>