---
title: 격리 상태 문제 해결
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7853"
- "9004348"
ms.openlocfilehash: 3ee932b7788f4aff3c8bc762c5c917124edfe065
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/22/2021
ms.locfileid: "49935400"
---
# <a name="troubleshoot-quarantine-state"></a><span data-ttu-id="f5bb2-102">격리 상태 문제 해결</span><span class="sxs-lookup"><span data-stu-id="f5bb2-102">Troubleshoot quarantine state</span></span>

<span data-ttu-id="f5bb2-103">Azure AD(Active Directory) 프로비전 서비스에서는 구성의 상태도 모니터링합니다.</span><span class="sxs-lookup"><span data-stu-id="f5bb2-103">The Azure Active Directory (AD) provisioning service monitors the health of your configuration.</span></span> <span data-ttu-id="f5bb2-104">또한 비정상 앱을 **격리** 상태에 둡니다.</span><span class="sxs-lookup"><span data-stu-id="f5bb2-104">It also places unhealthy apps in a **quarantine** state.</span></span> <span data-ttu-id="f5bb2-105">대상 시스템에 대해 거는 호출 중 대부분 또는 전체가 계속 실패하는 경우 프로비전 작업이 **격리** 로 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="f5bb2-105">If most, or all, of the calls made against the target system consistently fail, then the provisioning job is marked as **in quarantine**.</span></span> <span data-ttu-id="f5bb2-106">오류의 예로는 **유효하지 않은 관리자 자격 증명으로 인해 받은 오류** 가 있습니다. </span><span class="sxs-lookup"><span data-stu-id="f5bb2-106">An example of a failure is **an error received because of invalid admin credentials**.</span></span> <span data-ttu-id="f5bb2-107">자세한 내용은 [격리 상태의 응용 프로그램 프로비전](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-quarantine-status)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="f5bb2-107">For more information, see [Application provisioning in quarantine status](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-quarantine-status).</span></span>

<span data-ttu-id="f5bb2-108">클라우드 동기화 문제를 해결하려면 [격리된 문제 프로비전](https://docs.microsoft.com/azure/active-directory/cloud-sync/how-to-troubleshoot#provisioning-quarantined-problems)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="f5bb2-108">To troubleshoot cloud sync, see [Provisioning quarantined problems](https://docs.microsoft.com/azure/active-directory/cloud-sync/how-to-troubleshoot#provisioning-quarantined-problems).</span></span> 
