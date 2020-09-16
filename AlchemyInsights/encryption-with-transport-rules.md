---
title: 전송 규칙을 사용하여 암호화
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
- "9002635"
- "5154"
ms.openlocfilehash: 4c43fc16db84832c4e2aa3b6483632de6861b877
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47784349"
---
# <a name="encryption-with-transport-rules"></a>전송 규칙을 사용하여 암호화

[Exchange 관리 센터](https://go.microsoft.com/fwlink/p/?linkid=834822)(EAC)에서 메일 흐름 규칙의 Office 메시지 암호화(OME) 기능을 사용하여 메시지 암호화를 트리거할 수 있습니다. 전송 규칙 조건에서 **Office 365 메시지 암호화 및 권한 보호 적용** 옵션을 선택합니다.

- 자세한 내용은 [암호화를 위한 메일 흐름 규칙 정의](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)을 참조하세요.

- Powershell에서 [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) cmdlet을 사용하고 매개 변수 *ApplyOME*를 $true로 설정합니다.
