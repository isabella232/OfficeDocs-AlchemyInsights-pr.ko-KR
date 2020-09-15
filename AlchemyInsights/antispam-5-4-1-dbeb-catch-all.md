---
title: 스팸 방지 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717367"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>오류 코드 550 5.4.1 릴레이 액세스 거부에 대 한 배달 문제 수정

이 문제는 전자 메일 주소가 Microsoft 네트워크에 들어갈 때 [bouncebacks을 방지 하기 위해 유효한 지](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) 확인할 때 발생 합니다. 다음을 시도합니다.

1. 문제가 전체 도메인 또는 단일 전자 메일 주소에 적용 되는지 확인 합니다.
    - 전체 도메인: 도메인을 동기화 해야 하는 경우가 있습니다. [도메인을 Internal로 설정한 다음 다시 신뢰할](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)수 있도록 설정 해 봅니다.
    - 단일 전자 메일 주소: 주소를 동기화 해야 하는 경우도 있습니다. smtp 프록시 주소를 변경한 다음 다시 변경 하면 도움이 될 수 있습니다.
2. 문제가 그룹 또는 공용 폴더와 관련 된 것인지 확인 합니다. 일부 개체 유형의 경우 Azure Active Directory에서 개체를 수동으로 만들어야 할 수도 있습니다.

추가 도움이 필요한 경우 지원 티켓을 열고 문제 범위 (보내는 개체 유형 포함)를 지정 하 여 더 효율적으로 도움을 드릴 수 있습니다.