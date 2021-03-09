---
title: Mac에서 MDATP 설치 문제 해결
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
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568625"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="efb95-102">Mac에서 MDATP 설치 문제 해결</span><span class="sxs-lookup"><span data-stu-id="efb95-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="efb95-103">수동 설치가 실패하면 설치 마법사의 **요약** 페이지에 다음 오류가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="efb95-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="efb95-104">"설치하는 동안 오류가 발생했습니다.</span><span class="sxs-lookup"><span data-stu-id="efb95-104">"An error occurred during installation.</span></span> <span data-ttu-id="efb95-105">설치 관리자에서 오류가 발생하여 설치가 실패했습니다.</span><span class="sxs-lookup"><span data-stu-id="efb95-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="efb95-106">소프트웨어 제조업체에 문의하여 도움을 요청하세요."</span><span class="sxs-lookup"><span data-stu-id="efb95-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="efb95-107">MDM 배포의 경우 페이지에 일반 설치 실패도 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="efb95-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="efb95-108">최종 사용자에게 정확한 오류가 표시되지는는 않습니다. 설치 진행률이 있는 로그 파일은 **/Library/Logs/Microsoft/mdatp/install.log** 에 보관합니다.</span><span class="sxs-lookup"><span data-stu-id="efb95-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="efb95-109">각 설치 세션은 이 로그 파일에 추가됩니다.</span><span class="sxs-lookup"><span data-stu-id="efb95-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="efb95-110">마지막 설치 세션만 출력하기 위해 를 사용 `sed` 합니다.</span><span class="sxs-lookup"><span data-stu-id="efb95-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="efb95-111">자세한 내용은 [Mac용 Microsoft Defender ATP 설치 문제 해결을 참조합니다.](https://go.microsoft.com/fwlink/?linkid=2144615)</span><span class="sxs-lookup"><span data-stu-id="efb95-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
