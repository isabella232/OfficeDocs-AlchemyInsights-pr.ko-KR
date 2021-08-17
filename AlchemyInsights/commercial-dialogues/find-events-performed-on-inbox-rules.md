---
title: 받은 편지함 규칙에 대해 수행되는 이벤트 찾기
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: d6a4eadd897dfae3b65ccda6363edfe9cef1c810
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313505"
---
# <a name="find-events-performed-on-inbox-rules"></a>받은 편지함 규칙에 대해 수행되는 이벤트 찾기

받은 편지함 규칙을 만들거나 변경하거나 삭제하면 이벤트가 감사 로그에 기록됩니다. 검토하는 방법에는 다음이 있습니다.

1. 다음 작업 중 하나를 수행하십시오.
   - <https://compliance.microsoft.com>의 Microsoft 365 규정 준수 센터에서 **솔루션** \> **감사** 로 이동하세요. 또는 <https://compliance.microsoft.com/auditlogsearch>에서 **감사** 로 직접 이동하세요.
   - <https://security.microsoft.com>의 Microsoft 365 Defender에서 **감사** 로 이동하세요. 또는 <https://security.microsoft.com/auditlogsearch>에서 **감사** 로 직접 이동하세요.

    **참고:** 감사를 켜야 하다는 알림이 표시면 지금 진행하여 켜야 합니다. 이 기능을 설정하지 않은 경우 검색 결과에서 이전 날짜의 데이터를 끌 수 없습니다.
1. 활동 필드를 선택하고 Exchange 사서함 활동을 찾은 다음 New-InboxRule 받은 편지함 규칙 만들기를 Outlook Web App. 완료되면 창 외부를 클릭하여 활동 창을 최소화합니다.
1. 날짜 범위를 지정한 다음 사용자 필드에서 조사할 사용자의 사용자 이름을 선택합니다. 한에 두 개 이상의 사용자를 선택할 수 있습니다.
1. 검색을 선택합니다. 결과 아래에 활동들이 나타납니다.
1. 세부 정보를 확인하려면 활동을 선택한 다음 추가 정보를 선택합니다. 매개 변수 섹션에서는 규칙의 이름, 조건 집합 및 규칙이 수행할 작업을 볼 수 있습니다.

2. 감사 **페이지의 검색** **탭에서** 다음 설정을 구성합니다.
   - **날짜 및 시간 범위**: **시작** 및 **종료** 살자에서 날짜/시간 범위ㄹ르를 선택하세요.
   - **활동:** 새 **받은 편지함Rule** 목록에서 받은 편지함 규칙 Outlook Web App

3. 마쳤으면 **검색** 을 클릭합니다. 활동은 새 **검색 감사** 페이지에 표시됩니다.

4. 결과에서 활동을 선택하여 세부 정보 플라이아웃을 열 수 있습니다. 매개 **변수 섹션에서는** 규칙의 이름, 조건 집합 및 규칙이 수행할 작업을 볼 수 있습니다.

자세한 내용은 감사 로그 검색을 참조하여 일반적인 지원 [문제를 조사합니다.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
