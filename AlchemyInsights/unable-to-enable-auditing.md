---
title: 2419-사용할 수 없음 감사
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
ms.openlocfilehash: 81fd8e33feb2f2b10b04cc7cdc746a8603aa366b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767605"
---
# <a name="unable-to-enable-unified-auditing"></a>통합 감사를 사용 하도록 설정할 수 없음

조직에 대해 통합 감사를 사용 하도록 설정 하려고 하면 다음과 비슷한 오류가 표시 될 수 있습니다.

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

이 문제를 해결 하려면 다음 단계를 수행 합니다.

1. [Exchange Online Powershell에 연결](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)합니다.

2. 다음 cmdlet을 실행합니다.

   ```
   Enable-OrganizationCustomization
   ```

3. 이전 설정이 적용 되려면 60 분 정도 기다립니다.

4. Exchange Online PowerShell에서 다음 명령을 실행 합니다.

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

자세한 내용은 다음 문서를 참조 하십시오.

- [다단계 인증을 사용하여 Exchange Online PowerShell에 연결](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [감사 로그 검색 켜기 또는 끄기](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
