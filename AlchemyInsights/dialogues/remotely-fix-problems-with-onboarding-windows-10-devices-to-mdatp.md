---
title: Microsoft Defender Advanced Threat Protection에 Windows 10 장치 온보딩 문제를 원격으로 해결
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50530135"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a><span data-ttu-id="290d5-102">Microsoft Defender Advanced Threat Protection에 Windows 10 장치 온보딩 문제를 원격으로 해결</span><span class="sxs-lookup"><span data-stu-id="290d5-102">Remotely fix problems with onboarding Windows 10 devices to Microsoft Defender Advanced Threat Protection</span></span>

<span data-ttu-id="290d5-103">원격 컴퓨터에 액세스할 수 있는 경우 다음 단계를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="290d5-103">If you can access the remote computer, follow these steps:</span></span>

1. <span data-ttu-id="290d5-104">[클라이언트 연결 분석기](https://go.microsoft.com/fwlink/?linkid=2143466) 진단 도구를 다운로드합니다.</span><span class="sxs-lookup"><span data-stu-id="290d5-104">Download the [Client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466) diagnostic tool.</span></span>
2. <span data-ttu-id="290d5-105">MDATPAnalyzer.cmd를 압축 해제하고 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="290d5-105">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="290d5-106">분석기 도구를 다운로드한 폴더와 동일한 폴더인 MDATPClientAnalyzerResult 폴더에서 진단 로그를 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="290d5-106">Locate the diagnostic log in the MDATPClientAnalyzerResult folder, which is the same folder where the Analyzer tool was downloaded.</span></span>
4. <span data-ttu-id="290d5-107">연결 또는 인터넷 프록시 설정과 관련한 문제를 확인하려면 로그 파일 설정을 MDATPClientAnalyzer.txt.</span><span class="sxs-lookup"><span data-stu-id="290d5-107">To find issues with connectivity or Internet proxy settings, review the log file MDATPClientAnalyzer.txt.</span></span>

<span data-ttu-id="290d5-108">자세한 내용은 온보더링 [컴퓨터의 문제를 참조합니다.](https://go.microsoft.com/fwlink/?linkid=2143634)</span><span class="sxs-lookup"><span data-stu-id="290d5-108">To learn more, see [Issues with onboarding machines](https://go.microsoft.com/fwlink/?linkid=2143634).</span></span>
