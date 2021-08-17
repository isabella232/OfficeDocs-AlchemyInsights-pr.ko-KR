---
title: 618 일정 공유 정책
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: 1f1bfb0273301c05f5fe5f8af5fb9039328390d16305e33897680dce1c1977e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091609"
---
# <a name="policy-error-when-sharing-a-calendar"></a>일정을 공유할 때 정책 오류

1. 상황에 따라 다음 중 하나를 처리합니다.
    - 커넥트 PowerShell을 Exchange Online 사용하여 이 기능을 사용할 수 있습니다. 자세한 내용은 [원격 powerShell을 커넥트 Exchange Online 수 있습니다.를 참조하세요.](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)
    - On the on the on-premises server, open the Exchange Management Shell.
2. 사용자에게 할당된 공유 정책을 결정해야 합니다. 이렇게 하지 위해 다음 명령을 실행하고 반환된 정책을 메모합니다.

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. 사용자에 대한 공유 정책을 업데이트합니다. 이렇게 하려면 다음과 같이 하십시오.
    - Exchange 관리 센터를 엽니다.
    - 조직을 클릭한 다음 개별 공유에서 사용자에게 할당된 정책을 **두 번 클릭합니다.**  2단계에서 반환된 정책입니다.
    - 공유 규칙 페이지에서 공유할 정보 지정에서 허용할 일정 공유 수준을 **선택합니다.** 저장을 **클릭합니다.**

자세한 내용은 사용자가 일정을 공유하도록 할 때 "정책에서 이 수준의 사용 권한을 하나 이상의 받는 사람에게 부여할 수 없습니다." 오류를 [참조하세요.](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)
