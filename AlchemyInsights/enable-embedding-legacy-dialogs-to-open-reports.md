---
title: 보고서를 여는 데 기존 대화 포함 사용
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: 285933e607ac7e58256709f0c9cf2851250ce211
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806441"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="8fb5e-102">보고서를 여는 데 기존 대화 포함 사용</span><span class="sxs-lookup"><span data-stu-id="8fb5e-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="8fb5e-103">**증상**</span><span class="sxs-lookup"><span data-stu-id="8fb5e-103">**Symptom**</span></span>

<span data-ttu-id="8fb5e-104">사용자가 보고서를 열 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="8fb5e-104">Users are unable to open reports.</span></span> <span data-ttu-id="8fb5e-105">"문제가 발생했습니다.</span><span class="sxs-lookup"><span data-stu-id="8fb5e-105">"Something has gone wrong.</span></span> <span data-ttu-id="8fb5e-106">자세한 내용은 기술 세부 사항을 확인하세요."</span><span class="sxs-lookup"><span data-stu-id="8fb5e-106">Check technical details for more details."</span></span>

<span data-ttu-id="8fb5e-107">**원인**</span><span class="sxs-lookup"><span data-stu-id="8fb5e-107">**Cause**</span></span>

<span data-ttu-id="8fb5e-108">"양식 디스크립터가 NULL이거나 정의되지 않음" 오류와 함께 UCI에서 보고서를 로드하지 못했습니다.</span><span class="sxs-lookup"><span data-stu-id="8fb5e-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="8fb5e-109">UCI에서 보고서를 사용하려면 기존 대화가 계속 필요하므로, 고객의 시스템에 *allowlegacydialogsembedding*이 활성화되어 있어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="8fb5e-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="8fb5e-110">**솔루션**</span><span class="sxs-lookup"><span data-stu-id="8fb5e-110">**Solution**</span></span>

1. <span data-ttu-id="8fb5e-111">**설정 > 관리 > 시스템 설정 > 일반 탭**으로 이동합니다.</span><span class="sxs-lookup"><span data-stu-id="8fb5e-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="8fb5e-112">"통합 인터페이스 브라우저에서 특정 레거시 대화 포함 사용"을 **예**로 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="8fb5e-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
