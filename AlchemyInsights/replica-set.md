---
title: 복제 데이터베이스 집합
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50716273"
---
# <a name="replica-set"></a><span data-ttu-id="3abc2-102">복제 데이터베이스 집합</span><span class="sxs-lookup"><span data-stu-id="3abc2-102">Replica set</span></span>

<span data-ttu-id="3abc2-103">AADDS를 관리되는 도메인이라고도 합니다.</span><span class="sxs-lookup"><span data-stu-id="3abc2-103">AADDS is also called as the managed domain.</span></span> <span data-ttu-id="3abc2-104">실제로 백end에서 실행 및 유지 관리하는 도메인 컨트롤러 두 개입니다.</span><span class="sxs-lookup"><span data-stu-id="3abc2-104">It is actually two domain controllers that are run and maintained by the backend.</span></span> <span data-ttu-id="3abc2-105">두 개의 DC에는 하나의 주 DC와 하나의 복제 DC가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="3abc2-105">The two DCs include one main DC and one replication DC.</span></span> <span data-ttu-id="3abc2-106">AADDS(관리되는 도메인)의 백업은 Azure 플랫폼에서 관리하는 자동화된 프로세스입니다.</span><span class="sxs-lookup"><span data-stu-id="3abc2-106">Backups in AADDS (managed domain) are an automated process managed by the Azure platform.</span></span> <span data-ttu-id="3abc2-107">관리되는 도메인에 문제가 발생하면 Azure 지원이 백업에서 복원하는 데 도움이 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3abc2-107">In the event of an issue with your managed domain, Azure support can assist you in restoring from backup.</span></span>

<span data-ttu-id="3abc2-108">가상 네트워크에서 각 복제 데이터베이스 집합을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3abc2-108">You create each replica set in a virtual network.</span></span> <span data-ttu-id="3abc2-109">각 가상 네트워크는 관리되는 도메인의 복제본 집합을 호스트하는 다른 모든 가상 네트워크와 피어링되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="3abc2-109">Each virtual network must be peered to every other virtual network that hosts a managed domain's replica set.</span></span> <span data-ttu-id="3abc2-110">이 구성에서는 디렉터리 복제를 지원하는 메시 네트워크 토폴로지가 생성됩니다.</span><span class="sxs-lookup"><span data-stu-id="3abc2-110">This configuration creates a mesh network topology that supports directory replication.</span></span> <span data-ttu-id="3abc2-111">각 복제 데이터베이스 집합이 다른 가상 서브넷에 있는 경우 가상 네트워크에서 여러 복제 데이터베이스 집합을 지원할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3abc2-111">A virtual network can support multiple replica sets, provided that each replica set is in a different virtual subnet.</span></span>

<span data-ttu-id="3abc2-112">복제 데이터베이스 집합에 대한 자세한 내용은 개념 복제본 [집합 을 참조합니다.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)</span><span class="sxs-lookup"><span data-stu-id="3abc2-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span></span>
