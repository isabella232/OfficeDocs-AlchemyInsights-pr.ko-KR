---
title: 전송 규칙 수정
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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568561"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="4816b-102">전송 규칙 수정</span><span class="sxs-lookup"><span data-stu-id="4816b-102">Fix transport rules</span></span>

<span data-ttu-id="4816b-103">사용자 지정 메일 흐름 규칙이 이 메시지에 영향을 주었다.</span><span class="sxs-lookup"><span data-stu-id="4816b-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="4816b-104">정확한 규칙을 검토하기 위해 다음을 합니다.</span><span class="sxs-lookup"><span data-stu-id="4816b-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="4816b-105">제출 결과의 **추가 정보 아래에서** **GUID** 또는 정책 이름을 **메모합니다.**</span><span class="sxs-lookup"><span data-stu-id="4816b-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="4816b-106">Exchange 관리 셸을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="4816b-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="4816b-107">자세한 내용은 Exchange 관리 셸 [열기 를 참조하세요.](https://go.microsoft.com/fwlink/?linkid=2101432)</span><span class="sxs-lookup"><span data-stu-id="4816b-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="4816b-108">다음 명령을 실행합니다(제출의 GUID 사용): **Get-TransportRule -identity "GUID"** | fl \* Description\*</span><span class="sxs-lookup"><span data-stu-id="4816b-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="4816b-109">설명을 검토하여 메시지에 영향을 주는 구성된 조건을 검토합니다.</span><span class="sxs-lookup"><span data-stu-id="4816b-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="4816b-110">자세한 내용은 [Get-TransportRule 을 참조합니다.](https://go.microsoft.com/fwlink/?linkid=2101523)</span><span class="sxs-lookup"><span data-stu-id="4816b-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>
