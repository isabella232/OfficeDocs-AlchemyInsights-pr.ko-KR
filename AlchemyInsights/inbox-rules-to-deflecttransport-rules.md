---
title: 929 deflectTransport 규칙을 적용하는 받은 편지함 규칙
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
- "929"
- "1800021"
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: a143d36d1656e205311cde4aaff3c0c21815182ee82c60039b2219addac218cb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028658"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a>메일 흐름 규칙(전송 규칙)

- 메일 흐름 규칙의 일반 개요: 메일 흐름 [규칙(전송 규칙) Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)

- 메일 흐름 규칙 설정: 메일 흐름 규칙 [Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)

- 메일 흐름 규칙 만들기, 수정 및 삭제: [메일 흐름 규칙 관리](https://technet.microsoft.com/library/jj657505.aspx)

PowerShell에서 메일 흐름 규칙을 관리할 Exchange Online 있습니다. 자세한 내용은 [Get-TransportRule(보기),](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) [New-TransportRule(만들기),](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) [Remove-TransportRule(삭제),](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) [Set-TransportRule(기존](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) 수정), [Disable-TransportRule(기존](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) 사용 안 하도록 설정) 및 [Enable-TransportRule(기존](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) 사용 안 하도록 설정)을 참조하세요.

추가 메일 흐름 규칙 cmdlet: [Get-TransportRuleAction(사용](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) 가능한 작업 목록), [Get-TransportRulePredicate(사용](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) 가능한 조건 및 예외 목록), [Export-TransportRuleCollection(내보내기](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) 규칙) 및 [Import-TransportRuleCollection(가져오기](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) 규칙)
