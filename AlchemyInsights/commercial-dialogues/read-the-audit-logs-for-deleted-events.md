---
title: 삭제된 이벤트에 대한 감사 로그 읽기
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
ms.openlocfilehash: ec8f845f599e397814bc9077c3fe59edb5324192
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324739"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>삭제된 이벤트에 대한 감사 로그 읽기

이 작업을 하는 방법에는 다음이 있습니다.

1. 다음 작업 중 하나를 수행하십시오.
   - <https://compliance.microsoft.com>의 Microsoft 365 규정 준수 센터에서 **솔루션** \> **감사** 로 이동하세요. 또는 <https://compliance.microsoft.com/auditlogsearch>에서 **감사** 로 직접 이동하세요.
   - <https://security.microsoft.com>의 Microsoft 365 Defender에서 **감사** 로 이동하세요. 또는 <https://security.microsoft.com/auditlogsearch>에서 **감사** 로 직접 이동하세요.

    **참고:** 기능을 켜야 하다는 알림이 표시된 경우 앞으로 이동하여 지금 켜야 합니다. 기능이 켜져 있지 않은 경우 검색 결과에서 이전 날짜의 데이터를 끌어오지 못합니다.

2. 감사 **페이지의 검색** **탭에서** 다음 설정을 구성합니다.
   - **날짜 및 시간 범위**: **시작** 및 **종료** 살자에서 날짜/시간 범위ㄹ르를 선택하세요.
   - **활동**: Exchange **사서함 활동을 입력한** 후 다음 값을 선택합니다.
     - **지운 편지함 폴더에서 메시지 삭제됨**
     - **메시지가 지운 편지함 폴더로 이동됨**

       완료되면 창 외부를 클릭하여 활동 창을 **최소화합니다.**

   - **사용자**: 모든 사용자에 대한 결과를 반환하려면 빈 기본값을 그대로 사용하거나 한 명 이상의 사용자를 입력합니다.

3. 마쳤으면 **검색** 을 클릭합니다. 활동은 새 **검색 감사** 페이지에 표시됩니다.

4. 결과에서 활동을 선택하여 세부 정보 플라이아웃을 열 수 있습니다. 제목 줄 및 삭제된 항목의 위치와 같은 삭제된 항목에 대한 추가 정보가 **AffectedItems** 필드에 표시됩니다.

   **참고:** 감사 로그 기능을 사용하여 삭제된 항목은 복원할 수 없습니다. 삭제된 항목을 복원하려면 에서 삭제된 전자 메일 메시지 [복구를 웹용 Outlook.](https://support.microsoft.com/office/recover-deleted-email-messages-in-outlook-on-the-web-a8ca78ac-4721-4066-95dd-571842e9fb11)

자세한 내용은 감사 로그를 검색하여 일반적인 지원 [문제 조사를 참조하세요.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
