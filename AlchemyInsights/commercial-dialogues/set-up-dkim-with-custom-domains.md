---
title: 사용자 지정 도메인을 사용하여 DKIM 설정
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: c448956f0dad0738f4de7507ec4686c738a90a55
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736343"
---
# <a name="set-up-dkim-with-custom-domains"></a>사용자 지정 도메인을 사용하여 DKIM 설정

DNS의 각 사용자 지정 도메인에 대해 두 개의 CNAME 레코드를 게시해야 합니다. 이 작업을 위해 다음 형식을 사용 합니다.

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **DomainGUID는** 사용자 지정 도메인의 사용자 지정 MX 레코드에 있는 **.mail.protection.outlook.com** 왼쪽에 있는 텍스트입니다(예: 도메인 이름의 경우 contoso-com contoso.com).  **InitialDomain은** Office 365에 등록할 때 사용한 도메인입니다(예: contoso.onmicrosoft.com). 

DNS 레코드에 대한 자세한 내용은 [Office 365용 DNS](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)호스팅 공급자에서 DNS 레코드 만들기를 참조하세요.