---
title: 설치 DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808713"
---
# <a name="setup-dkim"></a>설치 DKIM

Microsoft 365에서 사용자 지정 도메인에 대 한 DKIM을 구성 하기 위한 전체 지침은 [여기](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)에 나와 있습니다.

1. **각** 사용자 지정 도메인에 대해 도메인의 DNS 호스팅 서비스 (대개 도메인 등록자)에서 **두 개의** dkim CNAME 레코드를 만들어야 합니다. 예를 들어 contoso.com 및 fourthcoffee.com에는 4 개의 DKIM CNAME 레코드 (contoso.com의 경우 2, fourthcoffee.com의 경우 2)가 필요 합니다.

   **각** 사용자 지정 도메인에 대 한 DKIM CNAME 레코드에는 다음과 같은 형식이 사용 됩니다.

   - **호스트 이름**: `selector1._domainkey.<CustomDomain>`

     **주소 또는 값을 가리킵니다**. `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **호스트 이름**: `selector2._domainkey.<CustomDomain>`

     **주소 또는 값을 가리킵니다**. `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> 은 `.mail.protection.outlook.com` 사용자 지정 도메인 (예: `contoso-com` contoso.com 도메인)에 대해 사용자 지정한 MX 레코드의 왼쪽에 있는 텍스트입니다. \<InitialDomain\> 은 Microsoft 365에 등록할 때 사용한 도메인 (예: contoso.onmicrosoft.com)입니다.

2. 사용자 지정 도메인에 대 한 CNAME 레코드를 만든 후에는 다음 지침을 따릅니다.

   a. 회사 또는 학교 계정으로 [Microsoft 365에 로그인](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) 합니다.

   b. 왼쪽 위에서 앱 시작 관리자 아이콘을 선택하고 **관리자**를 선택합니다.

   c. 왼쪽 아래 탐색에서 **관리자**를 확장하고 **Exchange**를 선택합니다.

   d. **보호**  >  **dkim**으로 이동 합니다.

   e. 도메인을 선택 하 고 **이 도메인에 대해 DKIM 서명을 사용 하 여 서명 메시지**에 대해 **사용** 을 선택 합니다. 각 사용자 지정 도메인에 대해 이 단계를 반복합니다.
