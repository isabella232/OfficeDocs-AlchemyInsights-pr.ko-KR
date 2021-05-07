---
title: 사용자용 추가 기능 Microsoft 365 앱
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233540"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="42f25-102">사용자용 추가 기능 Microsoft 365 앱</span><span class="sxs-lookup"><span data-stu-id="42f25-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="42f25-103">중앙 집중식 배포는 조직 내의 사용자 및 그룹에 Office 추가 기능을 배포하는 데 권장되는 방법입니다.</span><span class="sxs-lookup"><span data-stu-id="42f25-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="42f25-104">추가 기능을 배포하기 위해 다음 단계를 따르세요.</span><span class="sxs-lookup"><span data-stu-id="42f25-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="42f25-105">**참고:** 개별 사용자로 사용할 추가 기능을 Office 프로그램 에서 추가 기능 [보기, 관리 및 설치를 Office 참조합니다.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)</span><span class="sxs-lookup"><span data-stu-id="42f25-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="42f25-106">또한 스토어 추가 기능의 개별 Office 사용하도록 설정되어 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="42f25-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> <span data-ttu-id="42f25-107">자세한 내용은 모든 클라이언트에서 Office Store를 해제하여 추가 기능 다운로드 [방지(Outlook)를 참조합니다.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)</span><span class="sxs-lookup"><span data-stu-id="42f25-107">For details, see [Prevent add-in downloads by turning off the Office Store across all clients (Except Outlook)](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook).</span></span>

1. <span data-ttu-id="42f25-108">환경이 중앙 집중식 배포를 사용하여 추가 기능을 배포하기 위한 요구 사항을 충족하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="42f25-108">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="42f25-109">자세한 내용은 Requirements을 [참조하세요.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements)</span><span class="sxs-lookup"><span data-stu-id="42f25-109">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="42f25-110">통합 **설정** 추가 기능을 배포하려면 Microsoft 365 관리 센터에서 앱  >    >   다운로드로 이동하세요.</span><span class="sxs-lookup"><span data-stu-id="42f25-110">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="42f25-111">참고:</span><span class="sxs-lookup"><span data-stu-id="42f25-111">Notes:</span></span> 

- <span data-ttu-id="42f25-112">통합 앱을 사용하려면 관리자에게 전역 관리자 또는 관리자 권한이 Exchange 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="42f25-112">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="42f25-113">여러 사용자에게 추가 기능을 배포할 때 개별 사용자 대신 그룹을 사용하여 할당하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="42f25-113">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="42f25-114">자세한 내용은 사용자 및 그룹에 추가 기능을 할당할 때 고려 [사항을 참조합니다.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)</span><span class="sxs-lookup"><span data-stu-id="42f25-114">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="42f25-115">중앙 집중식 배포는 상위 그룹이 있는 중첩된 그룹 또는 그룹의 사용자를 지원하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="42f25-115">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="42f25-116">자세한 내용은 사용자 및 그룹 [할당을 참조합니다.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)</span><span class="sxs-lookup"><span data-stu-id="42f25-116">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="42f25-117">사용자가 로그인할 수 있도록 Microsoft 365 앱 관리 서비스(GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a')가 사용하도록 설정되어 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="42f25-117">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="42f25-118">자세한 내용은 앱 속성 [구성을 참조하세요.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)</span><span class="sxs-lookup"><span data-stu-id="42f25-118">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="42f25-119">통합 앱을 사용하여 추가 기능을 배포하는 데 문제가 있는 경우 추가 기능을 사용하여 [배포해 보아야 합니다.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)</span><span class="sxs-lookup"><span data-stu-id="42f25-119">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="42f25-120">자세한 내용은 다음을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="42f25-120">For more information, see:</span></span>

<span data-ttu-id="42f25-121">[관리 센터에서 추가 기능 배포](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [관리 센터에서 추가 기능 관리](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [중앙 집중식 배포 PowerShell cmdlet을](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 사용하여 추가 기능 관리 
 중앙 Office 센터를 통해 중앙 집중식 배포를 사용하여 Microsoft 365 [추가 기능 게시](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [문제 해결: 사용자가 추가 기능을 볼 수 없습니다.](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [추가 기능을 사용하여 사용자 Office 해결](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="42f25-121">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>