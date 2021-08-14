---
title: Dynamics 365 Forms 비즈니스 규칙 - 양식에 대해 비즈니스 규칙이 작성되지 않습니다.
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 8425918950e1ef6c44f2866e6fa8987fe165536ae21e08ea6a1da880f761d512
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53947305"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>필드가 프로그래밍식으로 변경된 경우 OnChange 이벤트가 발생하지 않습니다.

특성을 사용하여 필드를 프로그래밍식으로 변경하면 *OnChange* 이벤트가 발생하지 *않습니다.* [setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) 메서드 값을 설정한 후 *OnChange* 이벤트에 대한 이벤트 처리기에서 실행하려면 코드에서 *formContext.data.entity 특성* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) 메서드를 사용해야 합니다.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
