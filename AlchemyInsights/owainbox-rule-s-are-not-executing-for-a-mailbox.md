---
title: 1332 OWA - 사서함에 대해 받은 편지함 규칙이 실행되고 있지 않습니다.
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: b05ed9f0ee8c18b49b5338c53e67a79f1bf65464385dfa0ebd0639172a1b18f2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040908"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>받은 편지함 규칙이 예상대로 작동하지 않습니다.

다음 설정에서 웹용 Outlook.

- 받은 편지함 규칙에 따라 메시지를 한 번만 자동으로 리디렉션, 전달 또는 해당 메시지에 자동으로 보낼 수 있습니다. 리디렉션 규칙(전송 규칙라고도 하는 받은 편지함 규칙 또는 메일 흐름 규칙)은 메시지에 최대 10명의 전달 받는 사람을 추가할 수 있습니다. 자세한 내용은 저널, 전송 및 받은 편지함 [규칙 제한을 참조하세요.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)

- 받은 편지함 규칙은 대체 저널링 사서함에서 작동하지 않습니다. 대체 저널링 사서함에 대한 자세한 내용은 [Alternate journaling mailbox을 참조하십시오.](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)

이러한 문제를 해결하기 위해 [KB](https://support.microsoft.com/kb/2829319)2829319.

이전 문제가 적용되지 않는 경우 Microsoft 지원으로 에스컬레이터하기 전에 받은 편지함 규칙 진단 보고서를 실행합니다.

1. 사서함을 웹용 Outlook 다음을 클릭합니다. <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **설정**  >  **모든 Outlook 설정**  >  **메일**  >  **규칙**.

2. 페이지 아래쪽에서 규칙이 작동하지 않는 경우 여기를 클릭하여 진단 보고서를 **생성합니다.**
