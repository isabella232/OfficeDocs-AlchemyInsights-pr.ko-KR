---
title: Endpoint Manager - 보안 기준
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440890"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="05d85-102">Endpoint Manager - 보안 기준</span><span class="sxs-lookup"><span data-stu-id="05d85-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="05d85-103">보안 기준은 관련 보안팀에서 권장하는 보안 설정을 적용할 수 있도록 미리 구성된 Windows 설정 그룹입니다.</span><span class="sxs-lookup"><span data-stu-id="05d85-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="05d85-104">이러한 기준은 원하는 설정과 값만 제공하도록 사용자 지정될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="05d85-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="05d85-105">보안 기준에 대한 자세한 내용은 [보안 기준을 사용하여 Intune에서 Windows 10 장치 구성](https://docs.microsoft.com/mem/intune/protect/security-baselines)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="05d85-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="05d85-106">현재 다음 제품에 대한 기준이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="05d85-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="05d85-107">Windows MDM 보안 설정</span><span class="sxs-lookup"><span data-stu-id="05d85-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="05d85-108">엔드포인트용 Microsoft Defender  보안</span><span class="sxs-lookup"><span data-stu-id="05d85-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="05d85-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="05d85-109">Microsoft Edge</span></span>

<span data-ttu-id="05d85-110">각 기준은 주기적으로 업데이트되어 증분 버전으로 릴리스됩니다.</span><span class="sxs-lookup"><span data-stu-id="05d85-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="05d85-111">각 버전은 기준이 현재 지침을 충족하도록 이전 버전에서 설정을 추가하거나 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="05d85-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="05d85-112">Endpoint 보안의 보안 기준 콘솔을 사용하면 버전 간 변경 내용을 표시하여 서로 다른 버전을 비교할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="05d85-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="05d85-113">배포된 기준의 버전을 가장 효과적으로 변경하는 방법에 대한 지침은 [Microsoft Intune에서 보안 기준 프로필 관리](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="05d85-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="05d85-114">보안 기준을 배포한 후 배포 상태를 모니터링하고 장치 기준에 따라 설정을 검토할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="05d85-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="05d85-115">**참고:** 기준에 대한 데이터를 보고하는 경우 초기 배포에서 장치에 표시되는 데 최대 24시간, 추가 업데이트에 최대 6시간이 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="05d85-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="05d85-116">기준 설정이 적용되지 않는 가장 일반적인 원인은 다른 프로필에서 동일한 설정을 사용하기 때문입니다.</span><span class="sxs-lookup"><span data-stu-id="05d85-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="05d85-117">이 시나리오는 보안 기준 프로필의 장치 상태 노드에서 장치를 선택하여 특정 장치에 대해 조사할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="05d85-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="05d85-118">자세한 내용은 [보안 기준에 대한 충돌 해결](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="05d85-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>