---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821453"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="460f9-102">오류 코드 550 5.4.1 릴레이 액세스 거부에 대한 배달 문제 해결</span><span class="sxs-lookup"><span data-stu-id="460f9-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="460f9-103">이 문제는 전자 메일 [주소가](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) Microsoft 네트워크에 들어오면 반송을 방지할 수 있는 유효한지 확인할 때 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="460f9-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="460f9-104">다음을 시도합니다.</span><span class="sxs-lookup"><span data-stu-id="460f9-104">Try the following:</span></span>

1. <span data-ttu-id="460f9-105">문제가 전체 도메인 또는 단일 전자 메일 주소와 관련이 있는지 확인:</span><span class="sxs-lookup"><span data-stu-id="460f9-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="460f9-106">전체 도메인: 도메인을 동기화해야 하는 경우도 있습니다. 도메인을 내부로 설정한 다음 다시 권한을 [으로 설정해 보십시오.](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)</span><span class="sxs-lookup"><span data-stu-id="460f9-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="460f9-107">단일 전자 메일 주소: 주소를 동기화해야 하는 경우도 있습니다. smtp 프록시 주소를 변경한 다음 다시 변경하면 도움이 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="460f9-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="460f9-108">문제가 그룹 또는 공용 폴더와 관련이 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="460f9-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="460f9-109">일부 개체 유형의 경우 Azure Active Directory에서 개체를 수동으로 만들어야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="460f9-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="460f9-110">추가 도움이 필요한 경우 지원 티켓을 열고 문제의 범위(보내는 개체 유형 포함)를 지정하여 더 나은 지원을 제공하세요.</span><span class="sxs-lookup"><span data-stu-id="460f9-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>