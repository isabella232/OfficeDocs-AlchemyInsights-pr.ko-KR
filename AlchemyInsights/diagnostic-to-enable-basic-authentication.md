---
title: Exchange Online 프로토콜에 대한 기본 인증을 사용하기 위한 진단
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11392"
- "9006699"
ms.openlocfilehash: 25979df257d0534709f610b4d1547c52aeb269053c3d15a38969f15223b59e04
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993611"
---
# <a name="diagnostic-to-enable-basic-authentication-for-exchange-online-protocols"></a>Exchange Online 프로토콜에 대한 기본 인증을 사용하기 위한 진단

이 진단을 사용하면 POP3, IMAP4, Exchange ActiveSync, Exchange Web Services, 오프라인 주소록, MAPI, RPC 및 원격 PowerShell과 같은 Exchange Online 프로토콜에 대해 기본 인증을 사용하도록 설정할 수 있습니다. 이 인증은 Microsoft가 최근에 조직에서 사용하지 않도록 설정했을 수 있습니다. 

Microsoft는 테넌트가 사용하지 않기 때문에 환경에서 기본 인증을 해제할 준비가 된 곳을 알리기 위해 메시지 센터를 통해 직접 통신을 전송하여 관련 보안 위험으로부터 환경을 보호합니다.