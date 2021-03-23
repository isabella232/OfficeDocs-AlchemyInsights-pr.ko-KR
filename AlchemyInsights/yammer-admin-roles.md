---
title: 관리자 Yammer 정보를 제공합니다.
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003221"
- "9714"
ms.openlocfilehash: fd8534d44c44f2ea8e6b0de8c361109915566868
ms.sourcegitcommit: a6ab402f59e5ee1492bcf5ab7f18714fc251717d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/22/2021
ms.locfileid: "50995263"
---
# <a name="about-yammer-admins"></a><span data-ttu-id="ddd7d-102">관리자 Yammer 정보를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="ddd7d-102">About Yammer admins</span></span>

<span data-ttu-id="ddd7d-103">**네트워크 관리자**</span><span class="sxs-lookup"><span data-stu-id="ddd7d-103">**Network admins**</span></span>

<span data-ttu-id="ddd7d-104">전역 관리자는 전역 네트워크에서 확인된 관리자 역할로 Yammer 승격됩니다.</span><span class="sxs-lookup"><span data-stu-id="ddd7d-104">Global admins are automatically promoted to the Verified Admin role in a Yammer network.</span></span> <span data-ttu-id="ddd7d-105">다음 경우 이 승격이 제대로 발생하지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ddd7d-105">In the following cases, this promotion may not occur correctly:</span></span>

- <span data-ttu-id="ddd7d-106">여러 Yammer 네트워크가 있으며 관리자가 잘못된 네트워크로 로그인되고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ddd7d-106">Multiple Yammer networks exist, and the admin is being signed into the wrong one.</span></span> <span data-ttu-id="ddd7d-107">[네트워크 통합은](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) 하나의 네트워크로 Yammer 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="ddd7d-107">[Network consolidation](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) is required to get to one Yammer network.</span></span>
- <span data-ttu-id="ddd7d-108">Azure PIM이 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="ddd7d-108">Azure PIM is being used.</span></span> <span data-ttu-id="ddd7d-109">프로모션이 진행될 만큼 사용자가 전역 관리자로 승격되지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ddd7d-109">The user may not be promoted to global admin long enough for the promotion to occur.</span></span> <span data-ttu-id="ddd7d-110">이 Yammer 업데이트는 이 문제를 해결할 수 있지만 사용자를 전역 관리자로 수동으로 승격하는 것이 가장 좋은 것입니다.</span><span class="sxs-lookup"><span data-stu-id="ddd7d-110">A future update to Yammer may resolve this issue, but it is best to promote users to global admin manually.</span></span>
- <span data-ttu-id="ddd7d-111">동기화 네트워크에서 동기화 Yammer 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ddd7d-111">A sync issue exists with the Yammer network.</span></span> <span data-ttu-id="ddd7d-112">이 경우 추가 조사를 위해 지원 요청이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="ddd7d-112">In this case a support request will be required for further investigation.</span></span>

<span data-ttu-id="ddd7d-113">관리자 역할에 대한 Yammer 자세한 내용은 관리 관리자 [Yammer 참조하세요.](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins)</span><span class="sxs-lookup"><span data-stu-id="ddd7d-113">For more information about Yammer admin roles, see [Manage Yammer admins](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).</span></span>

<span data-ttu-id="ddd7d-114">**그룹 관리자**</span><span class="sxs-lookup"><span data-stu-id="ddd7d-114">**Group admins**</span></span>

<span data-ttu-id="ddd7d-115">Microsoft 365 연결된 그룹의 그룹 관리자는 Azure AD의 그룹 구성원과 동기화됩니다.</span><span class="sxs-lookup"><span data-stu-id="ddd7d-115">Group admins for Microsoft 365 connected groups are synced with group membership from Azure AD.</span></span> <span data-ttu-id="ddd7d-116">대규모 그룹의 경우 이 동기화에 시간이 더 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ddd7d-116">For large groups, this sync can take an extended period.</span></span>
