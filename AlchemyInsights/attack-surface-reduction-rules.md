---
title: 공격 노출 영역 축소 규칙
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/25/2021
ms.locfileid: "52651502"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="1e972-102">공격 노출 영역 축소 규칙</span><span class="sxs-lookup"><span data-stu-id="1e972-102">Attack surface reduction rules</span></span>

<span data-ttu-id="1e972-103">파일 또는 폴더를 제외하면 공격 표면 감소 규칙에서 제공하는 보호가 크게 감소할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1e972-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="1e972-104">규칙에 의해 차단된 파일은 실행할 수 있으며 보고서나 이벤트는 기록되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1e972-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="1e972-105">제외는 제외를 허용하는 모든 규칙에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="1e972-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="1e972-106">ASR 제외는 Microsoft Defender 바이러스 백신 제외와 동일한 구문을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="1e972-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="1e972-107">자세한 내용은 [Microsoft Defender 바이러스 백신 검색에 대한 제외 항목을 구성하고 확인](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1e972-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="1e972-108">문제를 방지하려면 [제외 항목을 정의할 때 피해야 할 일반적인 실수](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)를 검토하세요.</span><span class="sxs-lookup"><span data-stu-id="1e972-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="1e972-109">일부 ASR 규칙이 제외를 지원하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1e972-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="1e972-110">규칙이 제외를 지원하는지 확인하려면 [공격 표면 감소 규칙](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules) 표를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1e972-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="1e972-111">공격 노출 영역 축소 규칙</span><span class="sxs-lookup"><span data-stu-id="1e972-111">Attack surface reduction rules</span></span>

<span data-ttu-id="1e972-112">조직 공격 표면에는 공격자가 조직 장치 또는 네트워크를 손상시킬 수 있는 모든 장소가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="1e972-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="1e972-113">공격 표면을 줄이면 조직 장치와 네트워크를 보호할 수 있으므로 공격자가 공격을 수행할 수 있는 방법이 줄어듭니다.</span><span class="sxs-lookup"><span data-stu-id="1e972-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="1e972-114">엔드포인트용 Microsoft Defender에서 공격 표면 감소 규칙을 구성하면 도움이 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1e972-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="1e972-115">자세한 내용은 다음을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1e972-115">For more information, see:</span></span>

- [<span data-ttu-id="1e972-116">이름에 ASR 규칙 GUID 매핑</span><span class="sxs-lookup"><span data-stu-id="1e972-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="1e972-117">ASR 규칙 요구 사항:</span><span class="sxs-lookup"><span data-stu-id="1e972-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="1e972-118">Windows 10 Pro, 버전 1709 이상</span><span class="sxs-lookup"><span data-stu-id="1e972-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="1e972-119">Windows 10 Enterprise, 버전 1709 이상</span><span class="sxs-lookup"><span data-stu-id="1e972-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="1e972-120">Windows Server, 버전 1803(반기 채널) 이상</span><span class="sxs-lookup"><span data-stu-id="1e972-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="1e972-121">적용할 올바른 배제 식별</span><span class="sxs-lookup"><span data-stu-id="1e972-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="1e972-122">Microsoft-Windows-Windows Defender/Operational 로그에서 Look for eventID 1121 또는 1122를 조회합니다.</span><span class="sxs-lookup"><span data-stu-id="1e972-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="1e972-123">블록 시나리오와 컨텍스트를 평가하고 이 시나리오를 차단 해제해야 하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="1e972-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="1e972-124">이벤트 세부 정보에서 제외를 정의하는 값인 경로 값을 읽습니다.</span><span class="sxs-lookup"><span data-stu-id="1e972-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="1e972-125">가능한 한 엄격하게 제외합니다.</span><span class="sxs-lookup"><span data-stu-id="1e972-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="1e972-126">필요한 경우 와일드카드(예: 사용자 변수 바꾸기)를 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="1e972-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="1e972-127">배포 요구 사항에 따라 제외 항목을 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="1e972-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="1e972-128">자세한 내용은 [공격 표면 감소 규칙 사용자 정의](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1e972-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="1e972-129">제외는 존중되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="1e972-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="1e972-130">규칙이 제외를 지원하는지 여부를 결정합니다.</span><span class="sxs-lookup"><span data-stu-id="1e972-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="1e972-131">자세한 내용은 [공격 표면 감소 규칙](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1e972-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="1e972-132">적용된 제외 항목을 검토하고 이벤트 데이터로 오타 또는 잘못 해석된 와일드카드가 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="1e972-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="1e972-133">자세한 내용은 [지원되는 제외 규칙](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1e972-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="1e972-134">규칙의 영향이 너무 클 경우 추가 유효성 검사를 수행하기 위해 규칙을 감사 모드로 이동하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="1e972-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="1e972-135">자세한 내용은 [엔드포인트용 Microsoft Defender 기능이 감사 모드에서 작동하는 방식 테스트](/microsoft-365/security/defender-endpoint/audit-windows-defender)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1e972-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="1e972-136">다음 명령을 사용하여 지원 데이터를 수집하여 지원 사례를 엽니다.</span><span class="sxs-lookup"><span data-stu-id="1e972-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="1e972-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="1e972-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="1e972-138">자세한 내용은 [엔드포인트용 Microsoft Defender에 대한 시스템 온보드 관련 문제](issues-with-onboarding-machines.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1e972-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
