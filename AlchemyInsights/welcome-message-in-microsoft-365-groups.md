---
title: Microsoft 365 그룹의 환영 메시지
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
- "1200024"
- "5685"
ms.openlocfilehash: de16ca6021441bf6cb781106b7f3da8eed86b0f1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725845"
---
# <a name="welcome-message-in-microsoft-365-groups"></a>Microsoft 365 그룹의 환영 메시지

"UnifiedGroupWelcomeMessageEnabled" 속성이 True인 경우 Microsoft 365 그룹에 가입한 새 사용자는 환영 전자 메일을 받게 됩니다.

환영 메시지를 비활성화하려면 다음 [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) 명령을 사용합니다.

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
