---
title: 스팸 방지-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506449"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="cc38f-102">오류 코드 5.7.23에 대 한 전자 메일 배달 문제 해결</span><span class="sxs-lookup"><span data-stu-id="cc38f-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="cc38f-103">공개적으로 사용 가능한 SPF 또는 웹의 DNS 레코드 검사기에서 도메인에 대 한 SPF DNS 레코드를 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="cc38f-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="cc38f-104">아웃 바운드 메시지가 Microsoft의 스팸으로 식별 되지 않아 [위험성이 높은 배달 풀](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)을 통해 라우팅됩니다.</span><span class="sxs-lookup"><span data-stu-id="cc38f-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="cc38f-105">높은 위험 배달 풀의 메시지는 SPF 검사를 통과 하지 않으므로 대상 전자 메일 조직에서 허용 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="cc38f-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="cc38f-106">문제가 계속 되 면 전자 메일을 보내려고 시도 하는 메일 호스트의 관리자에 게 문의 해야 할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cc38f-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="cc38f-107">바운스 메시지에서 사용할 수 있는 자세한 외부 오류를 기록 합니다.</span><span class="sxs-lookup"><span data-stu-id="cc38f-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="cc38f-108">Microsoft support가 더 이상 지원 하지 않을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cc38f-108">Microsoft support may not be able to assist further.</span></span>
