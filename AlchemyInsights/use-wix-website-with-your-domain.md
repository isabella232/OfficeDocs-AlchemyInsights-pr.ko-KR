---
title: Office 365에서 구입했거나 관리되는 도메인으로 Wix 웹 사이트 사용
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
- "9001516"
- "3582"
ms.openlocfilehash: b45923ef112917fb95263dc2690672847129b05f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795061"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Office 365에서 구입했거나 관리되는 도메인으로 Wix 웹 사이트 사용

- [DNS 레코드를 업데이트하여 현재 호스팅 공급자에 웹 사이트 유지](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- Wix 문서 "포인팅 방법을 사용하여 Wix에 도메인 연결"에서는 Office 365를 사용할 때 네임 서버를 변경하는 대신 포인팅(위 링크당 DNS 레코드 추가)을 사용할 것을 권장합니다.
- 그럼에도 불구하고 이름 서버를 Wix로 변경하려면 [Microsoft용 Wix에서 DNS 레코드를 생성](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)해야 합니다.
- Microsoft에서 사용자의 도메인을 구입한 경우 이름 서버를 변경할 수 없습니다. 이름 서버를 변경해야 하는 경우 Microsoft에서 구입한 도메인을 [60일 후에 다른 호스팅 공급자로 이전](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)해야 할 것입니다.