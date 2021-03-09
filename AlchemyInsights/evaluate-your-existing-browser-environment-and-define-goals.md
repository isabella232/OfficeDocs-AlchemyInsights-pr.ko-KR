---
title: 기존 브라우저 환경을 평가하고 목표 정의
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9141"
- "9005291"
ms.openlocfilehash: 5b03d188aa78be83928cf262f1d86f3f933c85ab
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50530129"
---
# <a name="evaluate-your-existing-browser-environment-and-define-goals"></a><span data-ttu-id="66b1b-102">기존 브라우저 환경을 평가하고 목표 정의</span><span class="sxs-lookup"><span data-stu-id="66b1b-102">Evaluate your existing browser environment and define goals</span></span>

<span data-ttu-id="66b1b-103">시간을 내어 현재 브라우저 상태와 프로젝트 비전을 파악하면 모든 프로젝트 이해관계자가 조정되고 동일한 목표를 추구할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="66b1b-103">Taking time to understand your current browser state and project vision ensures all project stakeholders are aligned and are working toward the same goal.</span></span> <span data-ttu-id="66b1b-104">다음 단계를 따르세요.</span><span class="sxs-lookup"><span data-stu-id="66b1b-104">Follow these steps:</span></span>

1. <span data-ttu-id="66b1b-105">현재 상태를 정의합니다.</span><span class="sxs-lookup"><span data-stu-id="66b1b-105">Define your current state.</span></span> <span data-ttu-id="66b1b-106">다음과 같은 사항을 고려해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="66b1b-106">Consider the following:</span></span>
- <span data-ttu-id="66b1b-107">현재 환경에 배포된 브라우저는 무엇인가요?</span><span class="sxs-lookup"><span data-stu-id="66b1b-107">Which browsers are currently deployed in your environment?</span></span>
- <span data-ttu-id="66b1b-108">어떤 브라우저가 기본 브라우저로 설정되어 있나요?</span><span class="sxs-lookup"><span data-stu-id="66b1b-108">Which browser is set as the default browser?</span></span>
- <span data-ttu-id="66b1b-109">일부 앱에서 Internet Explorer를 사용해야 하나요?</span><span class="sxs-lookup"><span data-stu-id="66b1b-109">Do you need to use Internet Explorer for some of your apps?</span></span>
- <span data-ttu-id="66b1b-110">현재 엔터프라이즈 모드 사이트 목록을 사용하여 Internet Explorer를 구성하나요?</span><span class="sxs-lookup"><span data-stu-id="66b1b-110">Do you use an Enterprise Mode Site List to configure Internet Explorer today?</span></span>
- <span data-ttu-id="66b1b-111">환경이 Windows 10 및 macOS 등 어떤 OS 플랫폼을 지원하나요?</span><span class="sxs-lookup"><span data-stu-id="66b1b-111">Which OS platforms, such as Windows 10 and macOS, does your environment support?</span></span>
- <span data-ttu-id="66b1b-112">브라우저 관리에 어떤 관리 도구를 사용하나요?</span><span class="sxs-lookup"><span data-stu-id="66b1b-112">Which management tools do you use for browser management?</span></span>
- <span data-ttu-id="66b1b-113">브라우저 구성 및 관리를 담당하는 사람은 누구인가요?</span><span class="sxs-lookup"><span data-stu-id="66b1b-113">Who's responsible for browser configuration and management?</span></span>
- <span data-ttu-id="66b1b-114">브라우저 호환성을 검증하기 위한 프로세스는 무엇인가요?</span><span class="sxs-lookup"><span data-stu-id="66b1b-114">What's the process for validating browser compatibility?</span></span>
2. <span data-ttu-id="66b1b-115">배포의 목표를 정의합니다.</span><span class="sxs-lookup"><span data-stu-id="66b1b-115">Define the goals for your deployment.</span></span> <span data-ttu-id="66b1b-116">다음 사항도 유의해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="66b1b-116">Keep the following things in mind:</span></span>
- <span data-ttu-id="66b1b-117">[Microsoft Edge를 기본 브라우저로 설정](https://docs.microsoft.com/DeployEdge/edge-default-browser)하고 싶나요?</span><span class="sxs-lookup"><span data-stu-id="66b1b-117">Do you want to [set Microsoft Edge as your default browser](https://docs.microsoft.com/DeployEdge/edge-default-browser)?</span></span>
- <span data-ttu-id="66b1b-118">Microsoft Edge의 레거시 버전을 숨기고 싶나요? 아니면 [다른 사용자가 사용할 수 있도록 그대로](https://docs.microsoft.com/DeployEdge/microsoft-edge-sysupdate-access-old-edge) 두시겠어요?</span><span class="sxs-lookup"><span data-stu-id="66b1b-118">Do you want to hide the legacy version of Microsoft Edge or do you want to [leave it available for users](https://docs.microsoft.com/DeployEdge/microsoft-edge-sysupdate-access-old-edge)?</span></span>
- <span data-ttu-id="66b1b-119">[Microsoft Edge를 어떻게 구성](https://docs.microsoft.com/DeployEdge/configure-microsoft-edge)할 예정인가요?</span><span class="sxs-lookup"><span data-stu-id="66b1b-119">How will you [configure Microsoft Edge](https://docs.microsoft.com/DeployEdge/configure-microsoft-edge)?</span></span>
- <span data-ttu-id="66b1b-120">초기 배포의 일부로 구성하는 데 중요한 기능은 무엇인가요?</span><span class="sxs-lookup"><span data-stu-id="66b1b-120">What features are critical to configure as part of your initial deployment?</span></span>
- <span data-ttu-id="66b1b-121">식별된 호환성 또는 구성 문제를 해결하기 위한 프로세스는 무엇인가요?</span><span class="sxs-lookup"><span data-stu-id="66b1b-121">What is the process for addressing any identified compatibility or configuration issues?</span></span>
3. <span data-ttu-id="66b1b-122">다음과 같이 사용하려는 기능에 대한 필수 구성 요소를 이해하세요.</span><span class="sxs-lookup"><span data-stu-id="66b1b-122">Understand the prerequisites for features you might want to use, such as:</span></span>
- [<span data-ttu-id="66b1b-123">Windows Defender Application Guard</span><span class="sxs-lookup"><span data-stu-id="66b1b-123">Windows Defender Application Guard</span></span>](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-application-guard/reqs-md-app-guard)
- [<span data-ttu-id="66b1b-124">Internet Explorer 모드</span><span class="sxs-lookup"><span data-stu-id="66b1b-124">Internet Explorer mode</span></span>](https://docs.microsoft.com/DeployEdge/edge-ie-mode)
- [<span data-ttu-id="66b1b-125">인증 및 동기화</span><span class="sxs-lookup"><span data-stu-id="66b1b-125">Authentication and sync</span></span>](https://docs.microsoft.com/DeployEdge/microsoft-edge-security-identity)

<span data-ttu-id="66b1b-126">이러한 단계를 완료하고 나면 배포 전략을 계획할 준비가 된 것입니다.</span><span class="sxs-lookup"><span data-stu-id="66b1b-126">After you complete these steps, you're ready to start planning your deployment strategy.</span></span>
