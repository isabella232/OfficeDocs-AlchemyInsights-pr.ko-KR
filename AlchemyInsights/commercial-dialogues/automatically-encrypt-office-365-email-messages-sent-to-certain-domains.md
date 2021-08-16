---
title: 특정 도메인으로 Office 365 전자 메일 메시지를 자동으로 암호화
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 5a285f36aeb814e3b1d361c8cbffd5a6bef0770d10082d24654c7bbda59ce65b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082192"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>특정 도메인으로 Office 365 전자 메일 메시지를 자동으로 암호화

1. Exchange [관리 센터에서](https://outlook.office365.com/ecp/)메일 흐름 > **를 선택하세요.** 
2. 새로 **보기(+) 아이콘을** 클릭한 다음 메시지에 Office 365 메시지 암호화 및 권한 보호 적용을 **클릭합니다.**
3. 이름 **에** 규칙의 이름(예: 에 전송된 메시지 *암호화)을* contoso.com.
4. 다음의 경우 이 **규칙 적용에서** 받는 사람 > **를 선택 합니다.** 
5. 도메인 이름(예: 을(를) **contoso.com.**
6. **추가(+) 아이콘을** 클릭한 다음 확인을 **클릭합니다.**
7. 다음 작업을 **진행하십시오. 필드 옆에** 있는 하나 **선택을 클릭합니다.** 
8. **RMS 템플릿** 드롭다운 메뉴에서 **암호화를** 선택하고 확인 을 **클릭합니다.** (이 옵션이 없는 경우 요금제에 자동 암호화가 포함되어하지 않는 것입니다. 하지만 추가할 수 있습니다!)
9. 선택 사항(이 시점에서 만들 수 있는 선택 사항 목록에서 선택 사항 중 다수는 단순성을 위한 기본 설정으로 남을 수 있습니다)을 선택합니다.
10. **저장** 을 클릭합니다.

> [!IMPORTANT]
> 언제든지 돌아와서 나중에 이 규칙을 편집할 수 있습니다.

암호화 규칙을 만드는 데 대한 자세한 내용은 [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)