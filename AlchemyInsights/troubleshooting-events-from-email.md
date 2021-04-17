---
title: 전자 메일의 이벤트 문제 해결
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
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834845"
---
# <a name="troubleshooting-events-from-email"></a>전자 메일의 이벤트 문제 해결

1. 사서함에 대해 이 기능을 사용하도록 설정되었는지 확인합니다. **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. 그런 다음 '전자 메일의 이벤트' 로그 **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile** 을 확인합니다.

3. '전자 메일의 이벤트' 로그에서 사서함의 항목과 일치하는 InternetMessageId를 찾습니다.  

4. TrustScore는 항목이 추가되는지 여부를 결정합니다. TrustScore = "신뢰됨"인 경우에만 이벤트를 추가할 수 있습니다.

TrustScore는 메시지 머리글에 있는 SPF, Dkim 또는 Dmarc 속성에 따라 결정됩니다.

이러한 속성을 보려면 다음을 실행합니다.

**데스크톱 Outlook**

- 항목 열기
- 파일 -> 속성 -> 인터넷 머리글

또는

**MFCMapi**

- 받은 편지함에서 해당 항목으로 이동
- PR_TRANSPORT_MESSAGE_HEADERS_W 확인

이러한 속성은 전송과 라우팅을 수행하는 동안 결정되고 기록됩니다. 추가 문제 해결을 위해 SPF, DKIM 및/또는 DMARC의 오류에 대한 전송 지원을 추가해야 할 수 있습니다.