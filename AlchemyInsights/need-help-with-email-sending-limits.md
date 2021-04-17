---
title: 전자 메일 전송 제한 사항에 대한 도움이 필요한가요?
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
- "9002938"
- "5630"
ms.openlocfilehash: b5bdfbf818328c97ec93b3468aeedcbe88e03913
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836285"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="55890-102">전자 메일 전송 제한 사항에 대한 도움이 필요한가요?</span><span class="sxs-lookup"><span data-stu-id="55890-102">Need help with email sending limits?</span></span>

<span data-ttu-id="55890-103">다음은 서비스에 적용되는 **설계에 따른 제한** 입니다.</span><span class="sxs-lookup"><span data-stu-id="55890-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="55890-104">이러한 제한 사항에 대한 자세한 내용은 [여기](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits)에 문서로 정리되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="55890-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="55890-105">요청하지 않은 대량 메시지의 배달을 막기 위해 사용자별 **받는 사람 비율 제한을 모든 아웃바운드 및 내부 메시지** 에 적용합니다.</span><span class="sxs-lookup"><span data-stu-id="55890-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="55890-106">모든 SKU에서 이 제한은 **하루 10,000명의 받는 사람** 입니다.</span><span class="sxs-lookup"><span data-stu-id="55890-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="55890-107">적법한 상업성 대량 전자 메일(예: 고객 회보)을 보내려는 고객은 이러한 서비스를 제공하는 타사 제공업체를 이용해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="55890-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="55890-108">**참고**: 받는 사람 비율 제한에 도달하면 지난 24시간 내에 메시지를 받았던 받는 사람 수가 한도 미만이 될 때까지 사서함에서 메시지를 보낼 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="55890-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="55890-109">사용자는 그 시점까지 메시지를 보낼 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="55890-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="55890-110">**분당 30개의 메시지** 비율 제한이 모든 SKU에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="55890-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="55890-111">사용자가 지정된 기간 내에 Exchange Online 계정에서 보낼 수 있는 메시지 수를 결정합니다.</span><span class="sxs-lookup"><span data-stu-id="55890-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="55890-112">모든 SKU에서 단일 전자 메일 메시지에 대한 **받는 사람, 참조, 및 숨은 참조 필드에서 허용되는 최대 받는 사람의 수** 는 **1000명** 입니다.</span><span class="sxs-lookup"><span data-stu-id="55890-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="55890-113">이 제한을 사용자 지정하려면 [여기](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228)로 이동하세요.</span><span class="sxs-lookup"><span data-stu-id="55890-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
