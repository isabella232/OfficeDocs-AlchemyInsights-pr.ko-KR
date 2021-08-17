---
title: TLS 1.0 및 TLS 1.1 Office 365 때문에 전자 메일을 보내고 받을 수 없습니다.
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 508e48fd0e46557de075f4752da017ab8cc326923a965350140e598f7f7cf557
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054912"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>TLS 1.0 및 TLS 1.1 Office 365 때문에 전자 메일을 보내고 받을 수 없습니다.

메시지 센터 게시 MC229914에서 확인한 바에 따라 TLS 1.0 및 TLS 1.1 사용 중단이 메일 흐름 끝점에 Exchange Online 시작했습니다. 곧 Office 365 외부 원본의 TLS 1.0 및 TLS 1.1 전자 메일 연결을 더 이상 수락하지 않습니다. 또한 Exchange Online TLS 1.0 또는 1.1을 사용하여 아웃바운드 전자 메일을 보내지 않습니다. TLS 1.0 또는 1.1 비활성화로 문제가 발생하는 경우 다음 오류 중 하나를 경험할 수 있습니다.

- Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'
- 관리자 365- '421 4.4.2 SocketError로 인해 연결이 끊어졌다'에게 전자 메일을 보내는 On-Premises 서버의 큐 뷰어에서 오류가 발생했습니다.
- 송신 커넥터 [프로토콜](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) 로그에서 전자 메일을 보내는 서버의 Office 365- 오류 SocketError로 TLS 협상에 실패했습니다.
- 송신 또는 수신 커넥터 프로토콜 로그 오류 - '451 5.7.3 STARTTLS 명령을 먼저 실행해야 합니다'

위의 오류가 발생하는 경우 다음 레지스트리 키를 확인하여 전자 메일을 보내거나 받는 서버에 TLS 1.2가 사용하도록 설정되어 있는지 확인합니다.

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:00000001**

위의 레지스트리 키를 변경하여 TLS 1.2를 사용하도록 설정한 경우 서버를 다시 시작하여 변경 내용을 적용합니다. 또한 최신 업데이트 및 업데이트가 Windows Exchange 확인합니다.

자세한 내용은 다음 항목을 참조하세요.

- [Exchange Server TLS 지침, 1부: TLS 1.2 준비 - Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server TLS 지침 2부: TLS 1.2를 사용하도록 설정하고 사용하지 않는 클라이언트 식별 - Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Microsoft Tech Exchange Online TLS 버전에 동의할 수 없는 경우 전자 메일 시나리오 Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
