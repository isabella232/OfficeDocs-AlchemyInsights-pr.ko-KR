---
title: Linux 컴퓨터의 MDATP 제외 구성 및 유효성 검사
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
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568617"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a><span data-ttu-id="d143b-102">Linux 컴퓨터의 MDATP 제외 구성 및 유효성 검사</span><span class="sxs-lookup"><span data-stu-id="d143b-102">Configure and validate exclusions for MDATP on a Linux machine</span></span>

<span data-ttu-id="d143b-103">MDATP 검사에서 특정 파일, 폴더, 프로세스 및 처리된 파일을 제외할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d143b-103">You can exclude certain files, folders, processes, and process-opened files from MDATP scans.</span></span> <span data-ttu-id="d143b-104">제외는 조직에 고유하거나 사용자 지정된 소프트웨어 및 파일을 잘못 검색하지 못하도록 방지하는 데 도움이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="d143b-104">Exclusions help prevent incorrect detection of software and files unique or customized to your organization.</span></span> <span data-ttu-id="d143b-105">제외는 MDATP로 인한 성능 문제를 완화하는 데도 도움이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="d143b-105">Exclusions also help mitigate performance problems caused by MDATP.</span></span>

<span data-ttu-id="d143b-106">자세한 내용은 [Linux용 MDATP에](https://go.microsoft.com/fwlink/?linkid=2144517)대한 제외 구성 및 유효성 검사를 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="d143b-106">To learn more, see [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="d143b-107">이 문서에 설명된 제외는 끝점 감지 및 응답(EDR)을 포함하여 Linux용 MDATP의 다른 기능에는 적용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="d143b-107">The exclusions described in this article don't apply to other capabilities of MDATP for Linux, including endpoint detection and response (EDR).</span></span> <span data-ttu-id="d143b-108">이 문서에 설명된 방법을 사용하여 제외하는 파일은 여전히 EDR 경고 및 기타 검색 기능을 트리거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d143b-108">Files that you exclude by using the methods described in this article can still trigger EDR alerts and other detection capabilities.</span></span>
