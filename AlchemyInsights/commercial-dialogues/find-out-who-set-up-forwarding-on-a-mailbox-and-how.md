---
title: 사서함에 대해 전달을 설정하는 사람 및 방법 확인
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
ms.openlocfilehash: d6be4331967ed9ae362f5da85856b03cfa40b319
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317814"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>사서함에 대해 전달을 설정하는 사람 및 방법 확인

외부 전달이 사서함에 설정된 경우 **활동은 Set-Mailbox** cmdlet의 일부로 감사됩니다. 감사 로그에서 활동을 찾는 방법에는 다음이 있습니다.

1. 다음 작업 중 하나를 수행하십시오.
   - <https://compliance.microsoft.com>의 Microsoft 365 규정 준수 센터에서 **솔루션** \> **감사** 로 이동하세요. 또는 <https://compliance.microsoft.com/auditlogsearch>에서 **감사** 로 직접 이동하세요.
   - <https://security.microsoft.com>의 Microsoft 365 Defender에서 **감사** 로 이동하세요. 또는 <https://security.microsoft.com/auditlogsearch>에서 **감사** 로 직접 이동하세요.

   **참고:** 감사를 켜야 하다는 알림이 표시면 지금 진행하여 켜야 합니다. 이 기능을 설정하지 않은 경우 검색 결과에서 이전 날짜의 데이터를 끌 수 없습니다.

2. **감사** 페이지에서 **검색** 탭이 선택되었는지 확인하고 다음 설정을 구성하세요.
   - 시작 및 끝 상자에서  날짜/시간 범위를 선택합니다. 
   - 활동 **상자에** 모든 활동에 대한 결과 **표시가 포함되어 있는지 확인**

3. 마쳤으면 **검색** 을 클릭합니다. 활동은 새 **검색 감사** 페이지에 표시됩니다.

4. 결과에서 활동 **열을** 클릭하여 결과를 정렬하고 **Set-Mailbox 항목을** 검색합니다.

5. 결과에서 활동을 선택하여 세부 정보 플라이아웃을 열 수 있습니다. 활동이 전자 메일 전달과 관련이 있는지 확인하려면 각 감사 레코드의 세부 정보를 살펴보아야 합니다.
   - **ObjectId**: 수정된 사서함의 별칭 값입니다.
   - **매개** 변수: _ForwardingSmtpAddress는_ 대상 전자 메일 주소를 나타냅니다.
   - **UserId**: ObjectId 필드의 사서함에 대한 전자 메일 전달을 **구성한 사용자입니다.**

자세한 내용은 사서함에 대해 전자 [메일 전달을 설정한 사용자 확인을 참조하세요.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
