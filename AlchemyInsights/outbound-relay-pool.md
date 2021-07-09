---
title: 아웃바운드 릴레이 풀
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/08/2021
ms.locfileid: "53339981"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="7b321-102">아웃바운드 릴레이 풀</span><span class="sxs-lookup"><span data-stu-id="7b321-102">Outbound relay pool</span></span>

<span data-ttu-id="7b321-103">Microsoft는 사용자 계정을 통해 전자 메일을 릴레이하거나 전달하기 위한 구성을 Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="7b321-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="7b321-104">특정 시나리오의 메시지는 특수 릴레이 풀을 사용하여 Microsoft 365 릴레이됩니다.</span><span class="sxs-lookup"><span data-stu-id="7b321-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="7b321-105">릴레이 풀을 사용하여 보낸 메시지는 받는 사람의 정크 메일 폴더에 저장될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7b321-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="7b321-106">자세한 내용은 [아웃바운드 배달 풀을 참조하세요.](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span><span class="sxs-lookup"><span data-stu-id="7b321-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="7b321-107">릴레이 풀을 사용하는 시나리오를 피하기 위해 전달/릴레이된 메시지가 다음 조건 중 하나를 충족하는지 확인하십시오.</span><span class="sxs-lookup"><span data-stu-id="7b321-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="7b321-108">아웃바운드 보낸 사람이 테넌트의 허용 도메인입니다.</span><span class="sxs-lookup"><span data-stu-id="7b321-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="7b321-109">SPF(Sender Policy Framework)는 메시지가 전송되면 Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="7b321-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="7b321-110">P2 보낸 사람 도메인의 DKIM(DomainKeys Identified Mail)은 메시지가 전송될 때 Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="7b321-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="7b321-111">위의 조건을 충족하는 메시지는 릴레이 풀을 통해 릴레이되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="7b321-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="7b321-112">도메인의 MX 레코드가 타사 또는 사내 서버를 지정하는 경우 향상된 필터링을 사용하여 SPF 유효성 검사가 인바운드 전자 메일에 대해 올바른지와 릴레이 풀을 통해 전자 메일을 보내지 않도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="7b321-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="7b321-113">**릴레이 풀의 영향을 어떻게 알 수 있나요?**</span><span class="sxs-lookup"><span data-stu-id="7b321-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="7b321-114">전달되거나 릴레이된 전자 메일이 위의 조건 중 하나를 사용하는 경우 메시지는 릴레이 풀을 통해 릴레이되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="7b321-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="7b321-115">그러나 메시지가 릴레이 풀을 통해 전송되는 경우 아웃바운드 서버 IP는 40.95.0.0/16 범위에 있으며 아웃바운드 서버 이름에 **rly가** 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="7b321-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>

