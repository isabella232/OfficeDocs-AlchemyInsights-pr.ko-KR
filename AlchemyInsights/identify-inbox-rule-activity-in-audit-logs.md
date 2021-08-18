---
title: 감사 로그에서 받은 편지함 규칙 활동 식별
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1f252836d624b4550e1f3c87cf4fd7309dec6e91
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331129"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>감사 로그에서 받은 편지함 규칙 활동 식별

감사 로그 검색을 사용하여 받은 편지함 규칙 Microsoft 365 규정 준수 센터(받은 편지함 규칙 만들기, 수정 및 삭제)를 볼 수 있습니다.

1. 다음 단계 중 하나를 실행합니다.
   - <https://compliance.microsoft.com>의 Microsoft 365 규정 준수 센터에서 **솔루션** \> **감사** 로 이동하세요. 또는 <https://compliance.microsoft.com/auditlogsearch>에서 **감사** 로 직접 이동하세요.
   - <https://security.microsoft.com>의 Microsoft 365 Defender에서 **감사** 로 이동하세요. 또는 <https://security.microsoft.com/auditlogsearch>에서 **감사** 로 직접 이동하세요.

2. 감사 **페이지의 검색** **탭에서** 다음 설정을 구성합니다.
   - **날짜 및 시간 범위**: **시작** 및 **종료** 살자에서 날짜/시간 범위ㄹ르를 선택하세요.
   - **활동:** 다음 값 중 하나 이상을 선택합니다.
     - **New-InboxRule 사용자로부터 받은 편지함 규칙 Outlook Web App**
     - **Set-InboxRule 에서 규칙 Outlook Web App.**
     - **클라이언트에서 받은 편지함 Outlook 업데이트**

3. 마쳤으면 **검색** 을 클릭합니다. 활동은 새 **검색 감사** 페이지에 표시됩니다.

4. 결과에서 활동을 선택하여 세부 정보 플라이아웃을 열 수 있습니다. 받은 편지함 규칙 설정에 대한 정보가 매개 변수 **필드에** 표시됩니다.

자세한 내용은 [Determining if a user created an inbox rule 을 참조하십시오.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule)
