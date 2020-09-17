---
title: Project Online이 읽기 전용 상태입니다.
ms.author: pebaum
author: pebaum
manager: pamg
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1776"
- "9000205"
ms.openlocfilehash: ad2a9f95bf30708772edb166945f3f42e0f1f503
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801658"
---
# <a name="project-online-is-in-a-read-only-state"></a><span data-ttu-id="e76bd-102">Project Online이 읽기 전용 상태입니다.</span><span class="sxs-lookup"><span data-stu-id="e76bd-102">Project Online is in a read-only state</span></span>

<span data-ttu-id="e76bd-103">Project Online은 다음 세 가지 일반적인 이유로 인해 읽기 전용 상태가 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e76bd-103">There are three common reasons why Project Online may reach a read-only state:</span></span>

1. <span data-ttu-id="e76bd-104">조직은 Project Online Essentials 라이선스만 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="e76bd-104">Organizations have a Project Online Essentials license(s) only.</span></span> <span data-ttu-id="e76bd-105">이는 사이트를 유지 하 고 결국에는 프로 비전 되지 않도록 하기에 충분 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="e76bd-105">This isn't enough to keep the site alive and it will eventually get de-provisioned.</span></span><span data-ttu-id="e76bd-106">관리자에 게 어떤 것이 잘못 되어 올바른 라이선스를 획득할 수 있도록 사이트를 읽기 전용 상태로 설정 합니다.</span><span class="sxs-lookup"><span data-stu-id="e76bd-106"> We place the site in a read-only state so that Admins know something is wrong and can acquire the correct licenses.</span></span> <span data-ttu-id="e76bd-107">관리자에 게 Project Online Professional 및/또는 Premium 라이선스를 추가 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="e76bd-107">Admins will need to add a Project Online Professional and/or Premium license.</span></span> <span data-ttu-id="e76bd-108">사이트는 해당 시점에 읽기 전용으로 제공 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="e76bd-108">The site will come out of read-only at that point.</span></span> <span data-ttu-id="e76bd-109">자세한 내용은 [Compare Project Management Solutions](https://products.office.com/project/compare-microsoft-project-management-software?tab=1)를 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="e76bd-109">For more info, see [Compare Project Management Solutions](https://products.office.com/project/compare-microsoft-project-management-software?tab=1).</span></span>
2. <span data-ttu-id="e76bd-110">할당 된 할당량에 도달 했습니다.</span><span class="sxs-lookup"><span data-stu-id="e76bd-110">Assigned quota has been reached.</span></span> <span data-ttu-id="e76bd-111">자세한 내용은 [Project Web App 할당량](https://docs.microsoft.com/projectonline/tune-project-online-performance#project-web-app-quota)을 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="e76bd-111">For more info, see [Project Web App Quota](https://docs.microsoft.com/projectonline/tune-project-online-performance#project-web-app-quota).</span></span> <span data-ttu-id="e76bd-112">보고 세분성이 할당량 사용에 어떤 영향을 줄 수 있는지 보려면 [Project Online에서 시간대 별 보고 데이터 롤업을 구성을](https://docs.microsoft.com/ProjectOnline/configure-rollup-of-timephased-reporting-data-in-project-online) 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="e76bd-112">Check [Configure rollup of timephased reporting data in Project Online](https://docs.microsoft.com/ProjectOnline/configure-rollup-of-timephased-reporting-data-in-project-online) to see how reporting granularity may impact quota usage.</span></span>
3. <span data-ttu-id="e76bd-113">읽기 전용은 유지 관리 중에 발생할 수 있는 매우 일시적인 조건이 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e76bd-113">Read-only can be a very temporary condition that can occur during maintenance.</span></span> <span data-ttu-id="e76bd-114">대부분의 유지 관리는 고객의 의견을 제공 하지 않으며, 이러한 경우를 종종 볼 수는 없지만 읽기 전용 기간이 짧은 시간에 발생 하는 경우가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e76bd-114">Most maintenance is not even noticed by our customers and you will not often see this, but there are times when short periods of read-only are experienced.</span></span>
