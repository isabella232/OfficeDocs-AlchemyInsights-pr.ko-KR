---
title: 컴퓨터를 온보딩하는 데 문제 발생
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
ms.openlocfilehash: c3203ed68eb19d5f6d75eb2269094bb0422b14cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47676888"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="9d086-102">컴퓨터를 온보딩하는 데 문제 발생</span><span class="sxs-lookup"><span data-stu-id="9d086-102">Issues with onboarding machines</span></span>

<span data-ttu-id="9d086-103">MDATP 서비스에 컴퓨터를 온보딩하는 데 문제가 있을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="9d086-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="9d086-104">최종 사용자 컴퓨터에 액세스할 수 있는 경우 다음 단계를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="9d086-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="9d086-105">[클라이언트 연결 분석기](https://aka.ms/mdatpanalyzer) 진단 도구를 다운로드합니다.</span><span class="sxs-lookup"><span data-stu-id="9d086-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="9d086-106">MDATPAnalyzer.cmd를 압축 해제하고 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="9d086-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="9d086-107">분석 도구를 다운로드한 동일한 폴더에서 MDATPClientAnalyzerResult라는 진단 로그를 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="9d086-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="9d086-108">연결 또는 인터넷 프록시 설정 문제를 찾으려면 MDATPClientAnalyzer.txt 로그 파일을 검토합니다.</span><span class="sxs-lookup"><span data-stu-id="9d086-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>