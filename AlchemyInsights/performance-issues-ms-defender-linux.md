---
title: Linux의 엔드포인트용 Microsoft Defender 성능 문제
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783432"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="680f2-102">Linux의 엔드포인트용 Microsoft Defender 성능 문제</span><span class="sxs-lookup"><span data-stu-id="680f2-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="680f2-103">이 문서에서는 Linux의 엔드포인트용 Microsoft Defender에 대한 성능 문제를 식별하는 단계를 안내합니다.</span><span class="sxs-lookup"><span data-stu-id="680f2-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="680f2-104">먼저 발생한 문제가 [최신 버전](/microsoft-365/security/defender-endpoint/linux-whatsnew)으로 해결되었는지 확인하는 것이 중요합니다.</span><span class="sxs-lookup"><span data-stu-id="680f2-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="680f2-105">조사를 시작하려면 [Linux의 엔드포인트용 Microsoft Defender의 성능 문제 해결](/microsoft-365/security/defender-endpoint/linux-support-perf)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="680f2-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="680f2-106">제외</span><span class="sxs-lookup"><span data-stu-id="680f2-106">Exclusions</span></span>

<span data-ttu-id="680f2-107">제외는 성능 문제를 완화하는 데 도움이 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="680f2-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="680f2-108">추가 위험이 파악되고 문서화되도록 시작하기 전에 제외 사항을 검토하세요.</span><span class="sxs-lookup"><span data-stu-id="680f2-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="680f2-109">자세한 내용은 [Linux의 엔드포인트용 Microsoft Defender에 대한 제외 구성 및 유효성 검사](/microsoft-365/security/defender-endpoint/linux-exclusions)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="680f2-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="680f2-110">제외할 파일 및 폴더가 여러 개 있고 모두 동일한 마운트 지점에 있는 경우 마운트 지점을 제외하는 것이 더 쉬울 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="680f2-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="680f2-111">2월 릴리스 101.22.80부터 전체 마운트 지점을 제외할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="680f2-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="680f2-112">예를 들어 /mnt/backup이 마운트 지점인 경우 다음 명령을 실행하여 제외 목록에 /mnt/backup을 추가할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="680f2-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="680f2-113">**참고**: 제외 항목을 추가하면 맬웨어가 탐지되지 않을 위험이 증가하므로주의해서 처리하고 구현해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="680f2-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="680f2-114">도움이 필요하세요?</span><span class="sxs-lookup"><span data-stu-id="680f2-114">Need Help?</span></span>

<span data-ttu-id="680f2-115">가장 효율적인 방법으로 지원하려면 지원 케이스를 열기 전에 진단 데이터를 수집하세요.</span><span class="sxs-lookup"><span data-stu-id="680f2-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>
