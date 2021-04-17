---
title: 전송 규칙에서 DLP 사용
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: e512b36b34c5fc4931fb0f796790ee4b01c6443c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827222"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="8fe35-102">전송 규칙에서 DLP 사용</span><span class="sxs-lookup"><span data-stu-id="8fe35-102">Using DLP in transport rules</span></span>

<span data-ttu-id="8fe35-103">데이터 손실 방지(DLP) 기능을 기존의 전송에 통합하려면, 전송 규칙 설정에서 **메시지에 중요한 정보가 포함된 경우....."** 조건을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="8fe35-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="8fe35-104">**자세한 내용은 다음을 참조하세요.**</span><span class="sxs-lookup"><span data-stu-id="8fe35-104">**For more details, see:**</span></span>

- <span data-ttu-id="8fe35-105">전송 규칙에서의 통합 DLP 중요 정보 유형: [중요한 정보 규칙 통합](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="8fe35-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="8fe35-106">규칙에 대한 테스트 모드를 사용하여 정책 테스트를 사용하거나 사용하지 않고 규칙을 테스트할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8fe35-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="8fe35-107">규칙을 테스트하기 전에 만든 후 30분간 기다려야 합니다.</span><span class="sxs-lookup"><span data-stu-id="8fe35-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="8fe35-108">[메일 흐름/전송 규칙 테스트](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="8fe35-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="8fe35-109">**참고**: EAC에서 전송 규칙을 사용하여 새 DLP 정책을 구현하고자 하는 경우, [보안 및 규정 준수 센터](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide)를 대신 이용합니다.</span><span class="sxs-lookup"><span data-stu-id="8fe35-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
