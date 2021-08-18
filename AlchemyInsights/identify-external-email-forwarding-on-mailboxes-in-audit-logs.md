---
title: 감사 로그에서 사서함에 대한 외부 전자 메일 전달 식별
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
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 48634fad8f573e3a7c38cac299bb95ec90814f5c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331165"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>사서함에서 외부 전자 메일 전달이 구성된 경우 식별

사용자가 Microsoft 365 외부 전자 메일 전달을 구성하면 **활동이 Set-Mailbox** cmdlet의 일부로 감사됩니다. 감사 로그 검색을 사용하여 활동을 볼 수 있습니다. 이 작업을 하는 방법에는 다음이 있습니다.

1. 다음 단계 중 하나를 실행합니다.
   - <https://compliance.microsoft.com>의 Microsoft 365 규정 준수 센터에서 **솔루션** \> **감사** 로 이동하세요. 또는 <https://compliance.microsoft.com/auditlogsearch>에서 **감사** 로 직접 이동하세요.
   - <https://security.microsoft.com>의 Microsoft 365 Defender에서 **감사** 로 이동하세요. 또는 <https://sip.security.microsoft.com/auditlogsearch>에서 **감사** 로 직접 이동하세요.

2. **감사** 페이지에서 **검색** 탭이 선택되었는지 확인하고 다음 설정을 구성하세요.
   - 시작 및 끝 상자에서  날짜/시간 범위를 선택합니다. 
   - 활동 **상자에** 모든 활동에 대한 결과 **표시가 포함되어 있는지 확인**

3. 마쳤으면 **검색** 을 클릭합니다. 활동은 새 **검색 감사** 페이지에 표시됩니다.

4. 결과에서 **결과 필터링** 을 클릭하고 활동 필터링 상자에서 **Set-Mailbox** 를 입력하세요.

5. 결과에서 감사 레코드를 선택합니다. 세부 **정보** 플라이아웃에서 추가 정보를 **클릭합니다.** 활동이 전자 메일 전달과 관련이 있는지 확인하려면 각 감사 레코드의 세부 정보를 살펴보아야 합니다.

   - **ObjectId**: 수정된 사서함의 별칭 값입니다.
   - **매개** 변수: _ForwardingSmtpAddress는_ 대상 전자 메일 주소를 나타냅니다.
   - **UserId**: ObjectId 필드의 사서함에 대한 전자 메일 전달을 **구성한 사용자입니다.**

자세한 내용은 사서함에 대해 전자 [메일 전달을 설정한 사용자 확인을 참조하세요.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
