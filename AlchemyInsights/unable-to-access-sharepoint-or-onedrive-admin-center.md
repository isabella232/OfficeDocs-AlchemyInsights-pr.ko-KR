---
title: SharePoint 또는 OneDrive 관리 센터에 액세스할 수 없음
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: 7ba4a9c6995c03dd21e0e1aa387e407d41a08fb1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824441"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a><span data-ttu-id="507f7-102">SharePoint 또는 OneDrive 관리 센터에 액세스할 수 없음</span><span class="sxs-lookup"><span data-stu-id="507f7-102">Unable to access SharePoint or OneDrive admin center</span></span>

- <span data-ttu-id="507f7-103">SharePoint 또는 OneDrive 관리 센터 사이트에 액세스할 수 없거나 해당 사이트를 사용할 수 없는 경우, SharePoint 사이트 또는 OneDrive 콘텐츠에 액세스할 때 일시적인 지연이나 탐색 오류가 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="507f7-103">If your SharePoint or OneDrive Admin center site is inaccessible or unavailable, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="507f7-104">조직에 영향을 미치는지 확인하려면 [서비스 상태 대시보드](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)를 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="507f7-104">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

- <span data-ttu-id="507f7-105">전역 및 SharePoint 관리자에게 SharePoint 라이선스를 할당해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="507f7-105">Global and SharePoint admins need to be assigned a SharePoint license.</span></span> <span data-ttu-id="507f7-106">방금 SharePoint 라이선스 혹은 관리자 역할이 할당된 새로 만든 계정은 SharePoint에 액세스하는 데 "액세스가 거부됨" 또는 "사용자를 찾을 수 없음"과 같은 문제가 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="507f7-106">Newly created accounts just assigned with a SharePoint License or Admin role might experience issues accessing SharePoint, like "access denied" or "user not found."</span></span> <span data-ttu-id="507f7-107">시스템 전체에 동기화하는 데 최소 24시간을 기다려 주십시요.</span><span class="sxs-lookup"><span data-stu-id="507f7-107">Please give at least 24 hours for sync to complete across our systems.</span></span> <span data-ttu-id="507f7-108">24시간이 긴 것처럼 느껴질 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="507f7-108">We understand that 24 hours may seem like a long time.</span></span> <span data-ttu-id="507f7-109">대부분의 경우 당사는 이미 해결 방법에 대한 작업을 하고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="507f7-109">In many cases, we're already working on a solution.</span></span>

- <span data-ttu-id="507f7-110">허용된 액세스 시간이 매우 적은 경우, [PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)(Privileged Identity Management) 사용자가 액세스 거부됨 메시지를 받을 수 있습니다. [PIM 계정에 대한 액세스가 거부됨](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="507f7-110">Privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new))  users may receive access denied if allowed access time window is very small, see  [Access denied to PIM accounts](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).</span></span>