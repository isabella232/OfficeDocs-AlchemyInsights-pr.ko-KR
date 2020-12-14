---
title: Windows Virtual Desktop용 서비스 진단 도구
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/14/2020
ms.locfileid: "49665826"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="71b60-102">Windows Virtual Desktop용 서비스 진단 도구</span><span class="sxs-lookup"><span data-stu-id="71b60-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="71b60-103">WVD(Windows Virtual Desktop)는 관리자가 단일 인터페이스를 통해 오류를 식별할 수 있는 진단 도구를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="71b60-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="71b60-104">이 도구는 WVD 역할이 할당된 사용자가 WVD를 사용할 때마다 진단 관련 정보를 기록합니다.</span><span class="sxs-lookup"><span data-stu-id="71b60-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="71b60-105">각 로그에는 활동과 관련된 WVD 역할, 세션 중에 나타나는 오류 메시지 및 테넌트 및 사용자에 대한 정보가 포함되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="71b60-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="71b60-106">Azure Log Analytics는 진단 도구에서 만든 활동 로그를 캡처하도록 구성할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="71b60-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool.</span></span> <span data-ttu-id="71b60-107">방법은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="71b60-107">Here's how:</span></span>

1. <span data-ttu-id="71b60-108">Azure Portal 또는 [Azure PowerShell을](https://go.microsoft.com/fwlink/?linkid=2129501)사용하여 [Log](https://go.microsoft.com/fwlink/?linkid=2129500) Analytics 작업 영역 만들기</span><span class="sxs-lookup"><span data-stu-id="71b60-108">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>
1. <span data-ttu-id="71b60-109">[Windows 컴퓨터를 Azure Monitor에 연결합니다.](https://go.microsoft.com/fwlink/?linkid=2129913)</span><span class="sxs-lookup"><span data-stu-id="71b60-109">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="71b60-110">작업 영역의 기본 키와 작업 영역 ID를 얻습니다.</span><span class="sxs-lookup"><span data-stu-id="71b60-110">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="71b60-111">설치 마법사는 에이전트를 올바르게 구성하고 Azure Monitor와 통신할 수 있도록 이 정보가 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="71b60-111">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>
1. <span data-ttu-id="71b60-112">[진단 데이터를 작업 영역으로 푸시합니다.](https://go.microsoft.com/fwlink/?linkid=2128284)</span><span class="sxs-lookup"><span data-stu-id="71b60-112">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="71b60-113">WVD 테넌트의 진단 데이터를 작업 영역의 Log Analytics로 푸시할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="71b60-113">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>
1. <span data-ttu-id="71b60-114">[](https://go.microsoft.com/fwlink/?linkid=2128338) WVD와 관련한 내부 또는 외부 문제를 식별하고 진단합니다.</span><span class="sxs-lookup"><span data-stu-id="71b60-114">[Identify and diagnose issues](https://go.microsoft.com/fwlink/?linkid=2128338) that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="71b60-115">WVD용 서비스 진단 도구 구성에 대한 자세한 내용은 진단 기능에 [Log Analytics 사용을 참조하세요.](https://go.microsoft.com/fwlink/?linkid=2128084)</span><span class="sxs-lookup"><span data-stu-id="71b60-115">To learn more about configuring the service diagnostics tool for WVD, see [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span></span>
