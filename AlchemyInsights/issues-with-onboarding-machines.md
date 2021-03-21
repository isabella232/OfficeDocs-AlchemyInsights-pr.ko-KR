---
title: Microsoft Defender for Endpoint에 컴퓨터 온보딩 문제
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901573"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a><span data-ttu-id="156a2-102">Microsoft Defender for Endpoint에 컴퓨터 온보딩 문제</span><span class="sxs-lookup"><span data-stu-id="156a2-102">Issues with onboarding machines to Microsoft Defender for Endpoints</span></span>

<span data-ttu-id="156a2-103">MDE 서비스에 컴퓨터를 온보딩하는 데 문제가 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="156a2-103">You might have issues with onboarding machines to MDE service.</span></span> <span data-ttu-id="156a2-104">최종 사용자 컴퓨터에 액세스할 수 있는 경우 다음 단계를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="156a2-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="156a2-105">최신 미리 보기 버전의 [MDE 클라이언트 분석기](https://aka.ms/betamdeanalyzer) 진단 도구를 다운로드합니다.</span><span class="sxs-lookup"><span data-stu-id="156a2-105">Download the latest preview version of the [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="156a2-106">**MDEClientAnalyzer.cmd** 를 마우스 오른쪽 단추로 클릭하고 ‘관리자 권한으로 실행’을 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="156a2-106">Right click **MDEClientAnalyzer.cmd** and select ‘Run as administrator’.</span></span>
3. <span data-ttu-id="156a2-107">**MDEClientAnalyzer.htm** 의 제안된 지침을 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="156a2-107">Follow any guidance suggested in **MDEClientAnalyzer.htm**.</span></span>
4. <span data-ttu-id="156a2-108">자세한 로그는 **MDEClientAnalyzerResult** 라는 하위 폴더를 검토하세요.</span><span class="sxs-lookup"><span data-stu-id="156a2-108">For more verbose logs, review the created sub-folder named **MDEClientAnalyzerResult**.</span></span>
5. <span data-ttu-id="156a2-109">추가 지침이 필요한 경우, [엔드포인트용 Microsoft Defender 지원](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support)에 문의하고 분석을 위해 결과 MDEClientAnalyzerResult.zip 파일을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="156a2-109">If additional guidance is needed, contact [Microsoft Defender for Endpoint support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) and provide the resulting MDEClientAnalyzerResult.zip file for analysis.</span></span>
