---
title: " eDiscovery 보류 오류 문제 해결"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52583756"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a><span data-ttu-id="f8612-102"> eDiscovery 보류 오류 문제 해결</span><span class="sxs-lookup"><span data-stu-id="f8612-102">Troubleshooting ediscovery holds errors</span></span>

<span data-ttu-id="f8612-103">eDiscovery 보류에 문제가 있나요?</span><span class="sxs-lookup"><span data-stu-id="f8612-103">Experiencing issues with eDiscovery holds?</span></span> <span data-ttu-id="f8612-104">다음은 고려할 몇 가지 모범 사례입니다.</span><span class="sxs-lookup"><span data-stu-id="f8612-104">Here are some best practices to consider:</span></span>

- <span data-ttu-id="f8612-105">보류 배포 상태를 검사합니다.</span><span class="sxs-lookup"><span data-stu-id="f8612-105">Check the hold distribution status.</span></span>  <span data-ttu-id="f8612-106">상태가 **켜짐(보류 중)** 혹은 **꺼짐(보류 중)** 인 경우 보류 배포가 완료될 때까지 기다립니다.</span><span class="sxs-lookup"><span data-stu-id="f8612-106">If status is **On (Pending)** or **Off (Pending)**, wait for hold distribution to complete.</span></span>
- <span data-ttu-id="f8612-107">각 트랜잭션에 대해 정책을 반복적으로 업데이트하는 대신 eDiscovery 보류 업데이트를 단일 일괄 요청으로 병합합니다.</span><span class="sxs-lookup"><span data-stu-id="f8612-107">Merge eDiscovery hold updates into a single bulk request instead of updating the policy repeatedly for each transaction.</span></span>
- <span data-ttu-id="f8612-108">보안 및 준수 센터 PowerShell에서 Set-CaseHoldPolicy <policyname> -RetryDistribution을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="f8612-108">Run Set-CaseHoldPolicy <policyname> -RetryDistribution in the Security and Compliance Center Powershell.</span></span> <span data-ttu-id="f8612-109">자세한 내용은 [보안 및 준수 센터 PowerShell에 연결](/powershell/exchange/connect-to-scc-powershell)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="f8612-109">For details, see [Connect to Security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span></span>

<span data-ttu-id="f8612-110">이러한 설정 및 eDiscovery 보류 문제를 완화하고 해결하는 추가 모범 사례를 확인하기 위한 단계는 [eDiscovery 보류 오류 문제 해결](/microsoft-365/compliance/hold-distribution-errors)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="f8612-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span></span>
<span data-ttu-id="f8612-111">다른 일반적인 eDiscovery 문제 해결에 대한 자세한 내용은 [일반적인 eDiscovery 문제 조사, 문제 해결 및 해결](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="f8612-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span></span>
