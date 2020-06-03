---
title: 성능 문제-SharePoint 또는 OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 2dc0cd5f1641298853443d364eb9434ec1d9cd5a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511154"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="9e0b1-102">SharePoint 또는 OneDrive 느림, 액세스 불가 또는 여러 사용자가 사용할 수 없음</span><span class="sxs-lookup"><span data-stu-id="9e0b1-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="9e0b1-103">이전에 액세스 한 여러 사용자가 OneDrive 또는 SharePoint 사이트를 사용할 수 없는 경우 일시적인 서비스 문제가 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9e0b1-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="9e0b1-104">[서비스 상태 대시보드를 확인](https://portal.office.com/adminportal/home#/servicehealth)합니다.</span><span class="sxs-lookup"><span data-stu-id="9e0b1-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="9e0b1-105">**사용자 추가 및 라이선스를 허가 합니다.**</span><span class="sxs-lookup"><span data-stu-id="9e0b1-105">**Add and license the user**</span></span>

<span data-ttu-id="9e0b1-106">[비즈니스용 Microsoft 365에서 사용자에 게 라이선스를 할당](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="9e0b1-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="9e0b1-107">**사용 권한 할당**</span><span class="sxs-lookup"><span data-stu-id="9e0b1-107">**Assign Permissions**</span></span>

<span data-ttu-id="9e0b1-108">사용자에 게 Sharepoint 라이선스가 할당 되 고 여전히 액세스 거부 메시지를 수신 하는 경우에는 [해당 권한 수준이](https://docs.microsoft.com/sharepoint/understanding-permission-levels) 할당 되어 있는지 확인 하세요.</span><span class="sxs-lookup"><span data-stu-id="9e0b1-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="9e0b1-109">**액세스 요청 기능 사용 고려**</span><span class="sxs-lookup"><span data-stu-id="9e0b1-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="9e0b1-110">[액세스 요청 기능](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) 을 사용 하면 사용자가 현재 볼 수 있는 권한이 없는 콘텐츠에 대 한 액세스를 요청할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9e0b1-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="9e0b1-111">**사용자 지정 스크립트를 허용 하면 액세스 거부 문제가 발생할 수 있음**</span><span class="sxs-lookup"><span data-stu-id="9e0b1-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="9e0b1-112">*사용자 지정 스크립트 허용* 기능이 액세스 거부를 표시할 수 있는 몇 가지 시나리오가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9e0b1-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="9e0b1-113">영향을 받는 기능 목록, 보안 고려 사항 및 기능을 사용 하지 않도록 설정 하는 기능</span><span class="sxs-lookup"><span data-stu-id="9e0b1-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="9e0b1-114">[사용자 지정 스크립트 허용 또는 금지](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="9e0b1-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

