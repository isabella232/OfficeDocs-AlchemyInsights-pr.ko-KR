---
title: 2419-활성화할 수 없는 감사
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 0566a8d002b1bd9e38f3184824193394e49d56494d347338f96cfcdfdb758f4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007796"
---
# <a name="unable-to-enable-unified-auditing"></a>통합 감사를 사용하도록 설정할 수 없습니다.

조직에 대해 통합 감사를 사용하도록 설정하려고 하면 다음과 같은 오류가 표시될 수 있습니다.

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

이 문제를 해결하기 위해 다음 단계를 수행합니다.

1. [커넥트 Powershell을 Exchange Online 합니다.](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)

2. 다음 cmdlet을 실행합니다.

   ```
   Enable-OrganizationCustomization
   ```

3. 이전 설정이 적용될 때까지 60분 정도 기다립니다.

4. PowerShell에서 다음 Exchange Online 실행합니다.

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

자세한 내용은 다음 문서를 참조하세요.

- [다단계 인증을 사용하여 Exchange Online PowerShell에 연결](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [감사 로그 검색 켜기 또는 끄기](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
