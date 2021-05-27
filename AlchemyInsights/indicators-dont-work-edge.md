---
title: Edge 브라우저를 사용하여 표시기가 작동하지 않음
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
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/25/2021
ms.locfileid: "52651510"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="58aaa-102">Edge 브라우저를 사용하여 표시기가 작동하지 않음</span><span class="sxs-lookup"><span data-stu-id="58aaa-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="58aaa-103">표시기를 만든 후에는 Edge(Smartscreen)가 표시기를 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="58aaa-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="58aaa-104">자세한 내용은 [IP 및 URL/도메인 표시기 생성](/microsoft-365/security/defender-endpoint/indicator-ip-domain)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="58aaa-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="58aaa-105">1단계: 다음을 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="58aaa-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="58aaa-106">표시기가 올바른지 확인합니다(IP/URL에 오타가 없는지, 올바른 동작, 올바른 RBAC 그룹).</span><span class="sxs-lookup"><span data-stu-id="58aaa-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="58aaa-107">표시기를 만든 후 가능한 대기 시간을 고려하여 최소 2시간 동안 기다립니다.</span><span class="sxs-lookup"><span data-stu-id="58aaa-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="58aaa-108">시스템이 엔드포인트용 Microsoft Defender에 온보드되어 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="58aaa-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="58aaa-109">시스템이 클라우드와 통신할 수 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="58aaa-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="58aaa-110">[테스트 사이트](https://demo.smartscreen.msft.net)로 이동하여 Smartscreen이 활성화되어 있고 연결할 수 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="58aaa-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="58aaa-111">2단계: 잠재적인 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="58aaa-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="58aaa-112">클라이언트가 요구 사항을 충족하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="58aaa-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="58aaa-113">자세한 내용은 [IP 및 URL/도메인에 대한 지표 만들기](/microsoft-365/security/defender-endpoint/indicator-ip-domain)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="58aaa-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="58aaa-114">Edge 브라우저의 최신 버전을 실행 중인지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="58aaa-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="58aaa-115">최신 버전을 찾으려면 [내 Microsoft Edge 버전 확인](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="58aaa-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="58aaa-116">Edge 브라우저를 다시 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="58aaa-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="58aaa-117">표시기를 설정한 사이트로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="58aaa-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="58aaa-118">사이트가 예상대로 표시되지 않으면 3단계로 계속 진행합니다.</span><span class="sxs-lookup"><span data-stu-id="58aaa-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="58aaa-119">3단계: 데이터를 수집합니다.</span><span class="sxs-lookup"><span data-stu-id="58aaa-119">Step 3: Collect data</span></span>

- <span data-ttu-id="58aaa-120">**MDEClientAnalyzer** 진단 데이터를 수집합니다.</span><span class="sxs-lookup"><span data-stu-id="58aaa-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="58aaa-121">자세한 내용은 [엔드포인트용 Microsoft Defender로 시스템 온보드 문제 해결](issues-with-onboarding-machines.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="58aaa-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="58aaa-122">Fiddler 트레이스를 설치하고 수집하는 데 불편함이 없는 경우 [Telerik Fiddler](http://www.telerik.com/fiddler)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="58aaa-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="58aaa-123">Microsoft 지원의 지침을 원하는 경우 아래 지원 아이콘을 선택하여 지원 사례를 여세요.</span><span class="sxs-lookup"><span data-stu-id="58aaa-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>
