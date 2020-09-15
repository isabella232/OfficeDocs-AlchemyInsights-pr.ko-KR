---
title: SharePoint 또는 OneDrive에서 액세스 제한
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700461"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="f84f5-102">SharePoint 또는 OneDrive에서 액세스 제한</span><span class="sxs-lookup"><span data-stu-id="f84f5-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="f84f5-103">SharePoint Online/OneDrive 서비스에 대 한 액세스를 제한 하는 방법에는 여러 가지가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f84f5-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="f84f5-104">아래에는 다양 한 액세스 제한 방법이 설명 되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f84f5-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="f84f5-105">**사용 권한 제한**</span><span class="sxs-lookup"><span data-stu-id="f84f5-105">**Permission Restriction**</span></span>

<span data-ttu-id="f84f5-106">SharePoint Online 및 비즈니스용 OneDrive에서는 액세스 권한이 있는 그룹/개인 에게만 액세스 권한을 부여 하 여 사이트, 파일 및 폴더와 같은 항목에 대 한 액세스를 제한 합니다.</span><span class="sxs-lookup"><span data-stu-id="f84f5-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="f84f5-107">SharePoint 목록 또는 라이브러리에 대 한 사용 권한 사용자 지정</span><span class="sxs-lookup"><span data-stu-id="f84f5-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="f84f5-108">SharePoint 사이트 사용 권한 사용자 지정</span><span class="sxs-lookup"><span data-stu-id="f84f5-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="f84f5-109">하위 폴더의 사용 권한 변경</span><span class="sxs-lookup"><span data-stu-id="f84f5-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="f84f5-110">관리되지 않는 장치에서 액세스 제어</span><span class="sxs-lookup"><span data-stu-id="f84f5-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="f84f5-111">SharePoint 또는 전역 관리자로 서, 관리 되지 않는 장치 (예를 들어, Intune에서 하이브리드 AD에 연결 되거나 호환 되지 않는)에 대 한 SharePoint 및 OneDrive 콘텐츠 액세스를 차단 하거나 제한할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f84f5-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="f84f5-112">**네트워크 위치 제한**</span><span class="sxs-lookup"><span data-stu-id="f84f5-112">**Network Location Restriction**</span></span>

<span data-ttu-id="f84f5-113">IT 관리자는 사용자가 신뢰 하는 정의 된 네트워크 위치를 기반으로 SharePoint 및 OneDrive 리소스에 대 한 액세스를 제어할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f84f5-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="f84f5-114">이를  위치 기반 정책이라고도 합니다.</span><span class="sxs-lookup"><span data-stu-id="f84f5-114">This is also known as location-based policy.</span></span> <span data-ttu-id="f84f5-115">자세한 내용은 [네트워크 위치를 기반으로 SharePoint Online 및 OneDrive 데이터에 대 한 제어 액세스](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location) 를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="f84f5-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="f84f5-116">**사이트 잠금 제한**</span><span class="sxs-lookup"><span data-stu-id="f84f5-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="f84f5-117">SharePoint Online 내에서는 사이트 모음을 잠글 수 있으므로 아무도 액세스 하지 못합니다.</span><span class="sxs-lookup"><span data-stu-id="f84f5-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="f84f5-118">[Get-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState 속성을 사용 하 여 PowerShell 및 [SharePoint Online 관리 셸을](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) 통해이를 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f84f5-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="f84f5-119">**사용자가 사이트 또는 하위 사이트를 만들지 못하도록 제한**</span><span class="sxs-lookup"><span data-stu-id="f84f5-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="f84f5-120">SharePoint 관리자 또는 전역 관리자는 사용자가 자신의 SharePoint 사이트를 만들고 관리 하 고, 만들 수 있는 사이트 종류를 결정 하 고, 사이트의 위치를 지정 하도록 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f84f5-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="f84f5-121">자세한 내용은 [SharePoint Online에서 사이트 만들기 관리](https://docs.microsoft.com/sharepoint/manage-site-creation) 를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="f84f5-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

