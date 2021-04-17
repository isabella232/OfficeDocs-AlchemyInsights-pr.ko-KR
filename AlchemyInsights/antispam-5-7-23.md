---
title: Antispam - 5.7.23
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
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821417"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>오류 코드 5.7.23에 대한 전자 메일 배달 문제 해결

웹에서 공개적으로 사용할 수 있는 SPF 또는 DNS 레코드 검사기에서 도메인의 SPF DNS 레코드를 확인해야 합니다.

아웃바운드 메시지가 Microsoft에서 스팸으로 식별되지 않은지와 높은 위험 배달 풀을 통해 [라우팅되지 않는지 확인](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) 위험 배달 풀의 메시지는 SPF 검사를 통과하지 못하므로 대상 전자 메일 조직에서 수락되지 않습니다.

문제가 계속되면 전자 메일을 보내고 있는 메일 호스트의 관리자에게 문의해야 할 수 있습니다. 반송 메시지에서 자세한 외부 오류를 메모해 두어야 합니다. Microsoft 지원은 더 이상 지원하지 않을 수 있습니다.
