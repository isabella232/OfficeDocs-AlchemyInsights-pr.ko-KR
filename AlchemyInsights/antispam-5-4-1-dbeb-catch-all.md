---
title: AntiSpam 5.4.1 DBEB catch-all
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
- "9001209"
- "3167"
ms.openlocfilehash: e0e9b4fec0615943227f40043aeed842e8ee556c5916a59f65e79ce121ec9547
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932283"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>오류 코드 550 5.4.1 릴레이 액세스 거부에 대한 배달 문제 해결

이 문제는 전자 메일 [주소가](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) Microsoft 네트워크에 들어오면 반송을 방지할 수 있는 유효한지 확인할 때 발생합니다. 다음을 시도합니다.

1. 문제가 전체 도메인 또는 단일 전자 메일 주소와 관련이 있는지 확인:
    - 전체 도메인: 도메인을 동기화해야 하는 경우도 있습니다. 도메인을 내부로 설정한 다음 다시 권한을 [으로 설정해 보십시오.](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)
    - 단일 전자 메일 주소: 주소를 동기화해야 하는 경우도 있습니다. smtp 프록시 주소를 변경한 다음 다시 변경하면 도움이 될 수 있습니다.
2. 문제가 그룹 또는 공용 폴더와 관련이 있는지 확인합니다. 일부 개체 유형의 경우 개체 형식에서 개체를 수동으로 만들어야 할 수 Azure Active Directory.

추가 도움이 필요한 경우 지원 티켓을 열고 문제의 범위(보내는 개체 유형 포함)를 지정하여 더 나은 지원을 제공하세요.