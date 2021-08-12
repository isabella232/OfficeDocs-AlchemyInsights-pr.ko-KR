---
title: SpamHaus에서 차단된 전자 메일을 보내는 중 오류가 발생했습니다.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8372032e19bd2ebaf3ba8cc8e87f19ef3e2edf1e607b1739a919f6dcc443cd97
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946758"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>전자 메일 보내기 오류: Spamhaus를 사용하여 클라이언트 호스트가 차단되었습니다.

메시지를 보낸 IP 주소는 [Spamhaus가](https://go.microsoft.com/fwlink/p/?linkid=123245)소유한 차단 목록에 있습니다. Spamhaus가 차단하는 이유는 손상된 계정, 공용 IP 주소를 공유하는 손상된 컴퓨터 및 ISP(인터넷 서비스 공급자) 정책입니다. 가능한 해결 방법:
  
- 원본 전자 메일 서버를 제어하는 차단된 인바운드 메시지의 경우 원인을 파악하고 Spamhaus 웹 사이트에서 차단을 제거해야 합니다.

- 원본 IP 주소가 다른 사람에게 속하는 차단된 인바운드 메시지의 경우 주소 소유자는 Spamhaus 웹 사이트에서 차단을 제거해야 합니다. IP 주소가 PBL(정책 차단 목록)에 있는 경우 소유자는 다른 고정 IP 주소를 할당하거나 PBL에서 주소를 제거할 수 있습니다.

- Microsoft에 연결된 도메인에서 보낸 차단된 아웃바운드 메시지의 경우 메시지가 제3자 서비스를 통해 라우팅되는 경우 이 오류를 수신할 수 있습니다. WHOIS 검색 도구를 사용하여 차단된 IP 주소 소유자를 찾을 수 있습니다.
