---
title: DKIM 설정
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
ms.openlocfilehash: 5dc90965516cc4d360b9be56c7737c6d134123ea8ac263b092559dd1416faff4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54108562"
---
# <a name="setup-dkim"></a>DKIM 설정

에서 사용자 지정 도메인에 대해 DKIM을 구성하기 위한 전체 Microsoft 365 여기에 [있습니다.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

1. 각 **사용자** 지정 도메인에 대해 도메인의 DNS 호스팅 서비스(일반적으로 도메인 등록 기관)에 **두** 개의 DKIM CNAME 레코드를 만들어야 합니다. 예를 들어 contoso.com fourthcoffee.com DKIM CNAME 레코드 4개, contoso.com 2개, fourthcoffee.com.

   각 사용자 지정 도메인에  대한 DKIM CNAME 레코드는 다음 형식을 사용 합니다.

   - **호스트 이름**: `selector1._domainkey.<CustomDomain>`

     **주소 또는 값:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **호스트 이름**: `selector2._domainkey.<CustomDomain>`

     **주소 또는 값:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> 은 사용자 지정 도메인의 사용자 지정 MX 레코드 왼쪽에 있는 텍스트입니다(예: 도메인 레코드의 경우 `.mail.protection.outlook.com` `contoso-com` contoso.com. \<InitialDomain\>은 등록할 때 사용한 도메인입니다Microsoft 365(예: contoso.onmicrosoft.com.

2. 사용자 지정 도메인에 대한 CNAME 레코드를 만든 후 다음 지침을 완료합니다.

   a. [로그인하여 Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) 또는 학교 계정으로 로그인합니다.

   b. 왼쪽 위에서 앱 시작 관리자 아이콘을 선택하고 **관리자** 를 선택합니다.

   c. 왼쪽 아래 탐색에서 **관리자** 를 확장하고 **Exchange** 를 선택합니다.

   d. 보호   >  **DKIM으로 이동 합니다.**

   e. 도메인을 선택한 다음  DKIM 서명을 사용하여 이 도메인에 대해 메시지 서명 사용 **을 선택합니다.** 각 사용자 지정 도메인에 대해 이 단계를 반복합니다.
