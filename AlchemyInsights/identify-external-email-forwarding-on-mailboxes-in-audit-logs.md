---
title: 감사 로그의 사서함에 대 한 외부 전자 메일 전달 확인
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 592eb92e4b0fe0f9da2fa20bb93ffa4fbbb76662
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508958"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>사서함에 대해 외부 전자 메일 전달이 구성 된 시기 식별

Microsoft 365 사용자가 사서함에 대해 외부 전자 메일 전달을 구성 하면 해당 활동은 **설정 된 사서함** cmdlet의 일부로 감사 됩니다. 보안 & 준수 센터에서 감사 로그 검색을 사용 하 여 작업을 확인할 수 있습니다.

1. [Microsoft 365 보안 & 준수 센터](https://protection.office.com/)에 로그인 합니다.

2. **검색**  >  **감사 로그 검색** 페이지로 이동 합니다.

3. **시작 날짜** 및 **끝 날짜** 필드에서 날짜 범위를 선택 합니다. 사용자 이름을 지정할 필요는 없습니다. **모든 활동에 대 한 결과를 표시**하도록 **작업** 필드가 설정 되어 있는지 확인 합니다.

4. **검색**을 클릭합니다.

결과에서 **결과 필터링** 을 클릭 하 고 활동 필터 상자에 **Set-Mailbox** 를 입력 합니다. 결과에서 감사 레코드를 선택 합니다. **세부** 정보 플라이 아웃에서 **추가 정보**를 클릭 합니다. 각 감사 레코드의 세부 정보를 확인 하 여 해당 활동이 전자 메일 전달과 관련 되는지 확인 해야 합니다.

- **ObjectId**: 수정 된 사서함의 별칭 값입니다.

- **Parameters**: _ForwardingSmtpAddress_ 는 대상 전자 메일 주소를 나타냅니다.

- **UserId**: **ObjectId** 필드의 사서함에 대 한 전자 메일 전달을 구성한 사용자입니다.

자세한 내용은 [사서함에 대 한 전자 메일 전달을 설정한 사용자 결정](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)를 참조 하세요.
