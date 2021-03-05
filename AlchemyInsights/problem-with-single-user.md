---
title: 단일 사용자 문제
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
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50428827"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="eff58-102">단일 사용자 문제</span><span class="sxs-lookup"><span data-stu-id="eff58-102">Problem with single user</span></span>

- <span data-ttu-id="eff58-103">서비스에서 아직 사용자를 평가할 기회가 제공되지 않았기 때문에 사용자가 프로비전되지 않았을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="eff58-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="eff58-104">프로비전에 걸리는 시간 및 프로비저닝 구성 페이지의 진행률 표시줄에 대한 지침을 검토합니다.</span><span class="sxs-lookup"><span data-stu-id="eff58-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="eff58-105">추가 세부 정보 섹션에 지정된 상태가 사용자가 생성/업데이트/삭제된 날짜 이전인 경우 아직 사용자를 평가하지 않은 것입니다.</span><span class="sxs-lookup"><span data-stu-id="eff58-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="eff58-106">이 시나리오에서 가장 좋은 일은 프로비저닝 서비스가 완료될 때까지 기다리는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="eff58-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="eff58-107">이 서비스는 원본 시스템(클라우드 HR)의 사용자에 대한 변경 내용만 인식합니다.</span><span class="sxs-lookup"><span data-stu-id="eff58-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="eff58-108">Azure AD의 원본 시스템에서 변경을 감지하고 Active Directory로 흐름하기 위해 유효한 변경이 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="eff58-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="eff58-109">프로비저닝 서비스에서 사용자를 평가하고 프로비전하지 않는 것으로 결정했습니다.</span><span class="sxs-lookup"><span data-stu-id="eff58-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="eff58-110">특성 기반의 지정 필터를 설정한 경우 사용자가 지정한 조건을 충족하는지 확인</span><span class="sxs-lookup"><span data-stu-id="eff58-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="eff58-111">사용자가 대상 시스템에 이미 있으며 원본 및 대상 일치의 사용자 상태가 일치하는 경우 추가 작업을 수행하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="eff58-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="eff58-112">프로비저닝 서비스가 사용자를 프로비전하려고 했지만 실패했습니다.</span><span class="sxs-lookup"><span data-stu-id="eff58-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="eff58-113">이러한 시나리오의 경우 프로비저닝 로그의 문제 해결 및 권장 사항 탭을 검토합니다.</span><span class="sxs-lookup"><span data-stu-id="eff58-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="eff58-114">사용자의 필수 특성이 사내 Active Directory 또는 Azure AD에 누락될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="eff58-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="eff58-115">예를 들어 userPrincipalName 또는 sAMAccountName 생성 규칙이 올바른 값을 생성하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="eff58-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="eff58-116">일치하는 특성(일반적으로 employeeId)은 사내 Active Directory 또는 Azure AD의 고유 사용자에게는 해당되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="eff58-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="eff58-117">예를 들어 AD에 employeeId가 같은 두 사용자가 있으며 서비스에서 동일한 원본 항목에 대한 중복 대상 항목을 나타내는 오류 코드를 반환합니다.</span><span class="sxs-lookup"><span data-stu-id="eff58-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="eff58-118">단일 사용자 및 그룹에 대한 로그를 검토하려면 특정 사용자와의 문제 프로비저닝 로그 [검토를 참조합니다.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)</span><span class="sxs-lookup"><span data-stu-id="eff58-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
