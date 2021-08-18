---
title: 도메인 또는 전자 메일을 보낸 사람을 안전한 사용자로 표시해야 하나요?
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
- "9002921"
- "5673"
ms.openlocfilehash: afc865a7b91036bd2d982e21dce059a87e109e3e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58319954"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>도메인 또는 전자 메일을 보낸 사람을 안전한 사용자로 표시해야 하나요?

- **수신 허용 - 보낸 사람 목록의 사용은** 조직을 스팸, 피싱 및 스푸핑 공격에 노출시키기 때문에 권장하지 않습니다.
- 그러나 비즈니스 요구 사항이 있는 경우, **[메일 흐름 규칙](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** 을 사용할 것을 **권장** 합니다. 당사의 지침은 보낸 사람 인증(보내는 도메인이 스푸핑 공격을 당하고 있지 않은지 확인)을 확인합니다. 
    **참고**: 스팸 필터링에 대한 예외가 조직을 보안 공격에 노출시킬 수 있으므로, 안전한 보낸 사람 목록을 사용하여 가양성을 관리하는 것은 권장하지 않습니다. 사용자가 스팸 또는 정크 메일로 잘못 표시된 메시지를 받는 경우, **[메시지와 파일을 Microsoft에 보고하세요](https://protection.office.com/reportsubmission)**.
- 스팸 방지 정책에서 Outlook에서의 수신 허용 - 보낸 사람, 허용된 보낸 사람 목록 혹은 허용된 도메인 목록은 보낸 사람이 모든 스팸, 스푸핑, 피싱 보호, 보낸 사람 인증(SPF, DKIM, DMARC)을 우회하기 때문에 **사용하지 않아야 합니다**. 이 방법은 임시 테스트에서만 가장 잘 사용됩니다.
- "X-Forefront-Antispam-Report" 메시지 헤더(SFV:SFE, SFV:SKA, SFV:SKN)를 확인하여 특정 이메일이 스팸 방지 유효성 검사를 우회했는지 확인합니다. **[스팸 방지 메시지 헤더](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)** 를 참조하세요.
- Microsoft는 [기본적으로 고객의 보안](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)을 유지하려고 하기 때문에 일부 테넌트 재정의는 맬웨어 및 높은 신뢰도 피싱에 적용되지 않습니다. 이러한 재정의에는 다음이 포함됩니다. o 허용된 보낸 사람 목록 또는 허용된 도메인 목록(스팸 방지 정책) o Outlook 안전한 보낸 사람 o IP 허용 목록(연결 필터링) 
- 높은 신뢰도의 피싱 메시지가 필터링을 우회하도록 허용하는 유일한 재정의는 Exchange 메일 흐름 규칙(전송 규칙이라고도 함)입니다. 메일 흐름 규칙을 사용하여 필터링을 무시하려면 **[메일 흐름 규칙을 사용하여 메시지지의 SCL(스팸 신뢰도 수준) 설정](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)** 을 참조하세요.