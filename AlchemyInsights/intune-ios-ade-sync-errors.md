---
title: Apple 자동 장치 등록 동기화 오류
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
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448928"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="2c0e4-102">Apple 자동 장치 등록 동기화 오류</span><span class="sxs-lookup"><span data-stu-id="2c0e4-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="2c0e4-103">"오류 상태인 ADE/DEP 토큰이 하나 이상 있는 것으로 감지되었습니다.</span><span class="sxs-lookup"><span data-stu-id="2c0e4-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="2c0e4-104">영향을 받는 각 토큰에 대해 오류 상태가 확인될 때까지 ADE 기능이 예상대로 작동하지 않습니다."</span><span class="sxs-lookup"><span data-stu-id="2c0e4-104">Until the error state is resolved for each affected token, the ADE functionality will not work as expected.”.</span></span>

<span data-ttu-id="2c0e4-105">이 오류는 여러 가지 방법으로 매니페스트될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2c0e4-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="2c0e4-106">장치가 ABM/ASM에서 Intune으로 동기화되지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2c0e4-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="2c0e4-107">등록 프로필 할당이 실패할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2c0e4-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="2c0e4-108">장치가 ADE 등록을 완료하지 못했습니다.</span><span class="sxs-lookup"><span data-stu-id="2c0e4-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="2c0e4-109">장치 등록 > Apple 등록 프로그램 토큰에서 Intune > 보고된 > 동기화 **> 확인합니다.**</span><span class="sxs-lookup"><span data-stu-id="2c0e4-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span></span>

<span data-ttu-id="2c0e4-110">동기화 오류의 가장 일반적인 원인 중 하나는 현재 토큰의 만료입니다.</span><span class="sxs-lookup"><span data-stu-id="2c0e4-110">One of the most common causes of sync error is expiration of the current token.</span></span> <span data-ttu-id="2c0e4-111">대부분의 경우 영향을 받는 토큰을 갱신하면 문제가 해결됩니다.</span><span class="sxs-lookup"><span data-stu-id="2c0e4-111">In many cases,renewal of the affected token will resolve the issue.</span></span>

<span data-ttu-id="2c0e4-112">하나 이상의 토큰이 만료된 경우 다음 설명서를 참조하여 토큰을 적절하게 갱신할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2c0e4-112">If one or more of your tokens has expired,  see the following documentation to help you renew them as appropriate:</span></span>

[<span data-ttu-id="2c0e4-113">자동화된 장치 등록 토큰 갱신</span><span class="sxs-lookup"><span data-stu-id="2c0e4-113">Renew an Automated Device Enrollment token</span></span>](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

<span data-ttu-id="2c0e4-114">또한 다음 설명서를 참조하여 토큰 동기화 실패의 원인이 되는 다른 오류에 대한 잠재적인 수정을 볼 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2c0e4-114">In addition, you can see the following documentation to see potential remediations for other errors causing token synchronization failures:</span></span>

[<span data-ttu-id="2c0e4-115">iOS/iPadOS 및 macOS 자동화된 장치 등록 토큰에 대한 ABM/ASM 동기화 오류</span><span class="sxs-lookup"><span data-stu-id="2c0e4-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[<span data-ttu-id="2c0e4-116">iOS/iPadOS 및 macOS 자동화된 장치 등록 토큰에 대한 ABM/ASM 동기화 오류</span><span class="sxs-lookup"><span data-stu-id="2c0e4-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
