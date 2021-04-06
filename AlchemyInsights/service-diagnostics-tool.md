---
title: Windows Virtual Desktop용 서비스 진단 도구
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/05/2021
ms.locfileid: "51590300"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="9dc27-102">Windows Virtual Desktop용 서비스 진단 도구</span><span class="sxs-lookup"><span data-stu-id="9dc27-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="9dc27-103">WVD(Windows Virtual Desktop)는 관리자가 단일 인터페이스를 통해 오류를 식별할 수 있는 진단 도구를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="9dc27-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="9dc27-104">이 도구는 WVD 역할을 할당한 사용자가 WVD를 사용할 때마다 진단 관련 정보를 기록합니다.</span><span class="sxs-lookup"><span data-stu-id="9dc27-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="9dc27-105">각 로그에는 활동에 포함된 WVD 역할에 대한 정보, 세션 중에 나타나는 오류 메시지, 테넌트 및 사용자에 대한 정보가 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="9dc27-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="9dc27-106">Azure Log Analytics는 다음 단계를 수행하여 진단 도구가 생성한 작업 로그를 캡처하도록 구성할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9dc27-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool by following these steps:</span></span>

1. <span data-ttu-id="9dc27-107">[Azure Portal](https://go.microsoft.com/fwlink/?linkid=2129500) 또는 [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501)을 사용하여 Log Analytics 작업 영역을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="9dc27-107">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>

1. <span data-ttu-id="9dc27-108">[Windows 컴퓨터를 Azure Monitor에 연결합니다](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="9dc27-108">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="9dc27-109">작업 영역 ID와 작업 영역의 기본 키를 받습니다.</span><span class="sxs-lookup"><span data-stu-id="9dc27-109">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="9dc27-110">에이전트를 올바르게 구성하고 Azure Monitor와 통신할 수 있도록 하려면 설정 마법사에서 이 정보가 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="9dc27-110">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>

1. <span data-ttu-id="9dc27-111">[진단 데이터를 작업영역에 푸시합니다](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="9dc27-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="9dc27-112">WVD 테넌트에서 작업 영역의 진단 데이터를 Log Analytics에 푸시할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9dc27-112">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>

1. <span data-ttu-id="9dc27-113">WVD와 관련된내부 또는 외부 문제를 [식별하고 진단](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)합니다.</span><span class="sxs-lookup"><span data-stu-id="9dc27-113">[Identify and diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) issues that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="9dc27-114">WVD용 서비스 진단 도구를 구성하는 방법에 대한 자세한 내용은 진단 기능에 대한 Log Analytics 사용을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="9dc27-114">To learn more about configuring the service diagnostics tool for WVD, see Use Log Analytics for the diagnostics feature.</span></span>