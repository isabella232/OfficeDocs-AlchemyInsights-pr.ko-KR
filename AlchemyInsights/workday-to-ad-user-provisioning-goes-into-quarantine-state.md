---
title: AD 사용자 프로비전 작업일이 격리 상태로 변함
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430773"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a><span data-ttu-id="98213-102">AD 사용자 프로비전 작업일이 격리 상태로 변함</span><span class="sxs-lookup"><span data-stu-id="98213-102">Workday to AD User Provisioning goes into quarantine state</span></span>

<span data-ttu-id="98213-103">**AD 사용자 프로비전 작업일이 격리 상태로 변하고 AD에서 사용자가 생성되지 않음**</span><span class="sxs-lookup"><span data-stu-id="98213-103">**Workday to AD User Provisioning goes into quarantine state and no users are created in AD**</span></span>

<span data-ttu-id="98213-104">AD 사용자 프로비전 작업일 작업이 격리 상태로 변하고 감사 로그에 다음 오류 메시지를 포함한 내보내기 실패 이벤트가 표시됩니다. **오류: OperationsError-SvcErr: 작업 오류가 발생했으므로 디렉터리 서비스에서 이 포리스트 외부의 개체에 대한 추천을 발급할 수 없습니다**.</span><span class="sxs-lookup"><span data-stu-id="98213-104">The Workday to AD User Provisioning job has gone into quarantine state and the audit logs show export failure events with the error message **Error: OperationsError-SvcErr: An operation error occurred. No superior reference has been configured for the directory service. The directory service is therefore unable to issue referrals to objects outside this forest**.</span></span> <span data-ttu-id="98213-105">이 오류는 일반적으로 Active Directory 컨테이너 OU가 올바르게 설정되지 않았거나 **parentDistinguishedName** 에 사용된 식 매핑에 문제가 있는 경우에 나타납니다.</span><span class="sxs-lookup"><span data-stu-id="98213-105">This error usually shows up if the Active Directory Container OU is not set correctly or if there are issues with the Expression Mapping used for **parentDistinguishedName**.</span></span>

<span data-ttu-id="98213-106">**새 사용자** 매개 변수의 기본 OU에 오타가 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="98213-106">Check the Default OU for **New Users** parameter for typos.</span></span> <span data-ttu-id="98213-107">지정한 OU가 AD에 이미 존재하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="98213-107">Ensure that the specified OU already exists in your AD.</span></span> <span data-ttu-id="98213-108">특성 매핑에서 **parentDistinguishedName** 을 사용하는 경우 항상 AD 도메인 내의 알려진 컨테이너로 평가해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="98213-108">If you are using **parentDistinguishedName** in the attribute mapping, ensure that it always evaluates to a known container within the AD domain.</span></span> <span data-ttu-id="98213-109">감사 로그의 내보내기 이벤트에서 생성된 값을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="98213-109">Check the Export event in the audit logs to see the generated value.</span></span>

<span data-ttu-id="98213-110">자동 프로비전 작업일을 구성하는 방법에 대한 자세한 내용은 [자습서: 자동 사용자 프로비전 작업일 구성](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="98213-110">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>

