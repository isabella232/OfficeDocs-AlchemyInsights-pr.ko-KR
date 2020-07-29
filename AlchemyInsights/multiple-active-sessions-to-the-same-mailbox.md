---
title: 같은 사서함에 여러 활성 세션
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1836"
- "9000248"
ms.openlocfilehash: d2fd3f20346012baed21efd4900ca4cf73391d91
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431539"
---
# <a name="multiple-active-sessions-to-the-same-mailbox"></a><span data-ttu-id="b34a4-102">같은 사서함에 여러 활성 세션</span><span class="sxs-lookup"><span data-stu-id="b34a4-102">Multiple active sessions to the same mailbox</span></span>

<span data-ttu-id="b34a4-103">Exchange 리소스의 사용을 제어하기 위해 사서함에는 "예산"이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b34a4-103">To control usage of Exchange resources, a mailbox has a "budget."</span></span>

<span data-ttu-id="b34a4-104">예산을 초과하는 예외는 다음과 같은 경우에 트리거 할 수 있습니다만 다음과 같은 경우에만 트리거 할 수 있는 것은 아닙니다.</span><span class="sxs-lookup"><span data-stu-id="b34a4-104">The over-budget exception can be triggered by, but is not limited to, the following circumstances:</span></span>

- <span data-ttu-id="b34a4-105">같은 Outlook Web App 세션에서 몇 개의 브라우저 탭이 열렸습니다.</span><span class="sxs-lookup"><span data-stu-id="b34a4-105">A few browser tabs are opened within the same Outlook Web App session.</span></span>

- <span data-ttu-id="b34a4-106">몇 가지 활성 Outlook Web App이 동일한 사서함에 세션을 진행하고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="b34a4-106">A few active Outlook Web App sessions to the same mailbox.</span></span>

- <span data-ttu-id="b34a4-107">몇 가지 다른 클라이언트 응용 프로그램 (Outlook, Outlook Mobile, 타사 클라이언트 앱)은 동시에 사서함에 액세스 합니다.</span><span class="sxs-lookup"><span data-stu-id="b34a4-107">A few other client applications (Outlook, Outlook Mobile, a third party client app) access the mailbox at the same time.</span></span>

- <span data-ttu-id="b34a4-108">검색 요청을 실행하는 것과 같은 긴 실행 작업은 다른 활성 사서함 세션에서 수행됩니다.</span><span class="sxs-lookup"><span data-stu-id="b34a4-108">Long running operations, such as executing search requests, are performed from another active mailbox session.</span></span>

