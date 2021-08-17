---
title: 레거시 eDiscovery 도구 사용 중지
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 2e7f898ac1a9e9469f633192be18e2a3a362023c83c9e510593196b5a4a0daf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074680"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>레거시 eDiscovery 도구 사용 중지

Microsoft 365 준수 센터의 새로운 eDiscovery 기능 및 향상된 기능으로 인해 다음 레거시 eDiscovery 도구 및 명령줄은 몇 개월 후 사용 중지됩니다.

- [Exchange](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) 관리 센터의 Exchange. [](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds)

- eDiscovery Exchange Online 보류를 지원하는 In-Place PowerShell cmdlet을 In-Place 있습니다. 이러한 cmdlet은 *-MailboxSearch cmdlet으로 총체적으로 식별됩니다. 여기에는 다음 cmdlet이 포함됩니다.

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- PowerShell에서 [검색-Exchange Online](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet입니다.
- 웹 서비스 API의 Exchange 작업은 다음과 같습니다.
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**사용 중지 타임라인**:
- **2020년 7월 1일** 더 이상 새 검색 및 보류를 만들 수 없지만 기존 검색을 실행, 편집 및 삭제할 수 있습니다. Microsoft 지원은 EAC에서 In-Place eDiscovery & 지원하지 않습니다.
    
- **2020년 10월 1일** In-Place eDiscovery & EAC의 보류 기능은 읽기 전용 모드로 설정되어 기존 검색 및 보류만 제거할 수 있습니다.

**자세한 내용은 을 참조하세요.**

 - [레거시 eDiscovery 검색 및 보류를 Microsoft 365 규정 준수 센터](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [eDiscovery 도구의 사용 중지](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [eDiscovery 및 In-Place 보류에 In-Place FAQ](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



