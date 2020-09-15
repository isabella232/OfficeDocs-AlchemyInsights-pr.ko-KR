---
title: Intune에서 오래 된 장치 자동 정리
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 49a15132253c59189e343aeaa1c11d450b344896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715027"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="36b19-102">Intune에서 오래 된 장치 자동 정리</span><span class="sxs-lookup"><span data-stu-id="36b19-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="36b19-103">Intune에서는 관리자가 서비스에서 오래 된 장치를 제거한 후 90일에서 270일 사이의 시간 간격 구성을 허용 합니다.</span><span class="sxs-lookup"><span data-stu-id="36b19-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="36b19-104">조직 전체 설정이며 활성화 되면 즉시 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="36b19-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="36b19-105">설정을 초과 하는 기간 동안 Intune 서버에 체크인하지 않은 장치는 영구적으로 삭제됩니다.</span><span class="sxs-lookup"><span data-stu-id="36b19-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="36b19-106">**참고** MDM 장치 개체만 정리 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="36b19-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="36b19-107">EAS 단독 장치 개체는 제외 됩니다.</span><span class="sxs-lookup"><span data-stu-id="36b19-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="36b19-108">장치 정리 설정 및 해당 "상태"를 기준으로한 장치 삭제에 대한 자세한 내용은 다음을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="36b19-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="36b19-109">설정: **마지막 체크인 날짜 후 장치 삭제: 예(일부 특정 날짜 값 (N))**</span><span class="sxs-lookup"><span data-stu-id="36b19-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="36b19-110">설정에서 구성한 값(N)을 기준으로하여 마지막으로 체크인 된 장치가 지정된 날짜를 지나면 Intune에서 해당 장치를 삭제합니다.</span><span class="sxs-lookup"><span data-stu-id="36b19-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="36b19-111">설정: **마지막 체크인 날짜 이후 장치 삭제: 아니요**</span><span class="sxs-lookup"><span data-stu-id="36b19-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="36b19-112">장치가 인증 된지 180일이 지나고 갱신되지 않으면 장치가 삭제됩니다.</span><span class="sxs-lookup"><span data-stu-id="36b19-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="36b19-113">**참고** 두 경우 모두 장치가 Intune에 등록되어 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="36b19-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="36b19-114">등록은 Intune 서비스에 처음으로 장치를 체크인 할 때 이루어집니다.</span><span class="sxs-lookup"><span data-stu-id="36b19-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="36b19-115">장치가 Intune에 등록 되었지만 Intune 등록 장치가 되지 않는 경우 장치는 등록 후 270일 이내에 삭제됩니다.</span><span class="sxs-lookup"><span data-stu-id="36b19-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="36b19-116">(90일에 해당 장치가 해지 된 것으로 표시하고 향후 180일 이후에는 기록을 삭제합니다.)</span><span class="sxs-lookup"><span data-stu-id="36b19-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="36b19-117">현재 어떤 장치에도 Intune 콘솔에 장치 인증 만료 날짜를 설정하는 장치가 존재하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="36b19-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>