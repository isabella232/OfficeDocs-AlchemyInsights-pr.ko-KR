---
title: 레거시 eDiscovery 도구 만료
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 94cd2127240be5faacd397ba6255fdb16e364308
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/26/2020
ms.locfileid: "46902626"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>레거시 eDiscovery 도구 만료

Microsoft 365 준수 센터에서 새롭게 향상 된 eDiscovery 기능을 사용 하는 경우 다음과 같은 레거시 eDiscovery 도구 및 commandlets이 제공 되는 달에 폐기 될 수 있습니다.

- Exchange 관리 센터의 원본 [위치 eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) 및 [현재 위치 유지](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds)

- 원본 위치 eDiscovery 및 원본 위치 유지를 지 원하는 Exchange Online PowerShell cmdlet입니다. (이러한 cmdlet은 집합적으로 *-New-mailboxsearch cmdlet으로 식별 됩니다.) 여기에는 다음 cmdlet이 포함 됩니다.

    - [New-mailboxsearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [시작-New-mailboxsearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [New-mailboxsearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [New-mailboxsearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Exchange Online PowerShell의 [검색 사서함](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet
- Exchange 웹 서비스 API에서 다음 작업을 수행 합니다.
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v 1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**만료 시간**:
- **2020 년 7 월 1 일** 더 이상 새 검색 및 보류를 만들 수 없지만 기존 검색을 실행, 편집 및 삭제 하는 것은 위험 합니다. Microsoft Support는 EAC에서 원본 위치 eDiscovery & 보류를 더 이상 지원 하지 않습니다.
    
- **2020 년 10 월 1 일** 원본 위치 eDiscovery & EAC에서 유지 되는 기능은 읽기 전용 모드로 설정 되므로 기존 검색 및 보류만 제거할 수 있습니다.

**자세한 내용은 다음 항목을 참조**하십시오.

 - [레거시 eDiscovery 검색 및 보류를 Microsoft 365 준수 센터로 마이그레이션](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [eDiscovery 도구의 사용 중지](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [원본 위치 eDiscovery 및 현재 위치 유지 관련 Faq](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



