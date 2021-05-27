---
title: 끝점 DLP 구성
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657935"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="f1a61-102">끝점 DLP 구성</span><span class="sxs-lookup"><span data-stu-id="f1a61-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="f1a61-103">Microsoft 끝점 DLP를 사용하여 Windows 10 장치의 중요한 정보에 대한 DLP 보호 및 모니터링 기능을 확장할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f1a61-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="f1a61-104">장치를 장치 관리에 등록한 후 DLP 정책을 만들어 항목에 보호 작업을 적용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f1a61-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="f1a61-105">활동 탐색기를 사용하여 중요한 항목의 활동을 모니터링할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f1a61-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="f1a61-106">자세한 내용은 [장치 관리에 장치 등록](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="f1a61-106">For more info, see [Onboarding devices into device management](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="f1a61-107">끝점 DLP를 시작하려면 다음을 수행하세요.</span><span class="sxs-lookup"><span data-stu-id="f1a61-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="f1a61-108">해당 SKU/구독 라이선스가 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="f1a61-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="f1a61-109">자세한 내용은 [SKU/구독 라이선스](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="f1a61-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="f1a61-p103">장치 관리를 사용하도록 설정하고 등록 페이지에 액세스하거나 장치 모니터링을 설정/해제하는 데 필요한 권한을 확인합니다. 자세한 내용은 [권한](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="f1a61-p103">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring. For more info, see [Permissions](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="f1a61-112">장치 등록 절차를 따라 장치 관리에 장치를 등록합니다.</span><span class="sxs-lookup"><span data-stu-id="f1a61-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="f1a61-113">자세한 내용은 [장치 등록](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="f1a61-113">For more info, see [Onboarding devices](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="f1a61-114">DLP 정책을 만들어 중요한 항목을 보호합니다.</span><span class="sxs-lookup"><span data-stu-id="f1a61-114">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="f1a61-115">자세한 내용은 [끝점 DLP 정책 시나리오](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="f1a61-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="f1a61-116">Microsoft 끝점 DLP에 대한 자세한 내용은 [Microsoft 365 끝점 데이터 손실 방지(미리 보기) 알아보기](/microsoft-365/compliance/endpoint-dlp-learn-about)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="f1a61-116">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="f1a61-117">**지원이 필요한 경우 중요한 데이터 수집 단계:**</span><span class="sxs-lookup"><span data-stu-id="f1a61-117">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="f1a61-118">[MDATP 클라이언트 분석기 미리 보기](https://aka.ms/betamdatpanalyzer)를 다운로드합니다.</span><span class="sxs-lookup"><span data-stu-id="f1a61-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span></span>
1. <span data-ttu-id="f1a61-119">cmd 창에서 도구를 관리자로 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="f1a61-119">Run the tool as Admin from the cmd window:</span></span>

    <span data-ttu-id="f1a61-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span><span class="sxs-lookup"><span data-stu-id="f1a61-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span></span>

1. <span data-ttu-id="f1a61-121">**추적을 수집할 시간(분) 입력:** 메시지가 표시되면 시나리오를 실행하는 데 필요한 시간(분)을 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="f1a61-121">When prompted with **Enter the number of minutes to collect traces:**, enter the number of minutes required to run the scenario.</span></span>
1. <span data-ttu-id="f1a61-122">시나리오를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="f1a61-122">Run the scenario.</span></span>

<span data-ttu-id="f1a61-123">지원 에이전트에 제공할 Zip 파일 출력을 수집합니다.</span><span class="sxs-lookup"><span data-stu-id="f1a61-123">Collect the Zip file output to give to the Support agent.</span></span>
