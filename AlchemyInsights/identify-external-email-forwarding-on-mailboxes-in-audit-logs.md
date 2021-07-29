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
ms.openlocfilehash: b7146b2b09b6ac1e33b192dcbcbfb72ea2593313
ms.sourcegitcommit: 89d938a2d402791ae66dddadba3063e9418f48cb
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/28/2021
ms.locfileid: "53630255"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>사서함에서 외부 전자 메일 전달이 구성된 경우 식별

사용자가 Microsoft 365 외부 전자 메일 전달을 구성하면 **활동이 Set-Mailbox** cmdlet의 일부로 감사됩니다. 감사 로그 검색을 사용하는 활동은 보안 및 준수 센터에서 & 있습니다.

1. Microsoft 365 [센터에 로그인합니다.](https://protection.office.com/)

2. 검색 감사 **로그 검색**  >  **페이지로** 이동합니다.

3. 시작 날짜 및  종료 날짜 필드에서 날짜 범위를 **선택합니다.** 사용자 이름을 지정할 필요가 없습니다. 활동 **필드가** 모든 활동에 대한 결과 **표시로 설정되어 있는지 확인**

4. **검색** 을 클릭합니다.

결과에서 결과 **필터링을** 클릭하고 활동 필터 상자에 **Set-Mailbox를** 입력합니다. 결과에서 감사 레코드를 선택합니다. 세부 **정보** 플라이아웃에서 추가 정보를 **클릭합니다.** 활동이 전자 메일 전달과 관련이 있는지 확인하기 위해 각 감사 레코드의 세부 정보를 살펴보아야 합니다.

- **ObjectId**: 수정된 사서함의 별칭 값입니다.

- **매개** 변수: _ForwardingSmtpAddress는_ 대상 전자 메일 주소를 나타냅니다.

- **UserId**: ObjectId 필드의 사서함에 대한 전자 메일 전달을 **구성한 사용자입니다.**

자세한 내용은 사서함에 대해 전자 [메일 전달을 설정한 사용자 확인을 참조하세요.](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
