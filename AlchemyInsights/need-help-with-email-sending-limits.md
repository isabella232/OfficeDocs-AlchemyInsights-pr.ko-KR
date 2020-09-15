---
title: 전자 메일 전송 제한 사항에 대한 도움이 필요한가요?
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
- "9002938"
- "5630"
ms.openlocfilehash: 66ff82afd7b44ef5fd4943bfc794c2fa35bbfa9e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702369"
---
# <a name="need-help-with-email-sending-limits"></a>전자 메일 전송 제한 사항에 대한 도움이 필요한가요?

다음은 서비스에 적용되는 **설계에 따른 제한**입니다. 이러한 제한 사항에 대한 자세한 내용은 [여기](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits)에 문서로 정리되어 있습니다.

- 요청하지 않은 대량 메시지의 배달을 막기 위해 사용자별 **받는 사람 비율 제한을 모든 아웃바운드 및 내부 메시지**에 적용합니다. 모든 SKU에서 이 제한은 **하루 10,000명의 받는 사람**입니다.  적법한 상업성 대량 전자 메일(예: 고객 회보)을 보내려는 고객은 이러한 서비스를 제공하는 타사 제공업체를 이용해야 합니다.
    - **참고**: 받는 사람 비율 제한에 도달하면 지난 24시간 내에 메시지를 받았던 받는 사람 수가 한도 미만이 될 때까지 사서함에서 메시지를 보낼 수 없습니다. 사용자는 그 시점까지 메시지를 보낼 수 없습니다.
- **분당 30개의 메시지** 비율 제한이 모든 SKU에 적용됩니다. 사용자가 지정된 기간 내에 Exchange Online 계정에서 보낼 수 있는 메시지 수를 결정합니다.
- 모든 SKU에서 단일 전자 메일 메시지에 대한 **받는 사람, 참조, 및 숨은 참조 필드에서 허용되는 최대 받는 사람의 수**는 **1000명**입니다. 이 제한을 사용자 지정하려면 [여기](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228)로 이동하세요.
