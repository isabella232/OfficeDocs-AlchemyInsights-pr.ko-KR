---
title: 사서함에 대한 자동 회신 설정
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 03c530e7ce5f00fce2222cf9993930b97e5a2818
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715135"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>사용자 사서함에 대한 자동 회신 설정

**메서드 1**

1. Microsoft 365 포털에 로그인합니다.

2. **사용자> 활성 사용자**(또는 공유 사서함에서 설정한 경우 **그룹> 공유 사서함**)로 이동하세요.

3. Microsoft Exchange 사서함이 있는 사용자를 선택하세요.

4. 바로 가기 메뉴에서 **메일 설정 > 자동 회신**(공유 사서함 인 경우 바로 가기에서 **자동 회신** 클릭)으로 이동합니다.

**메서드 2**

1. 관리자 자격 증명을 사용하여 Microsoft 365 관리 포털에 로그인합니다.

2. **관리 센터**를 확장하고 **Exchange**를 클릭합니다.

3. 오른쪽 상단에서 그림을 클릭하고 **다른 사용자**를 클릭한 다음, 변경할 사용자 사서함을 선택하세요.

4. 왼쪽에서 **옵션**을 선택하고 **전자 메일 구성**을 클릭한 다음 **자동 회신**을 클릭합니다.

**메서드 3**

Exchange Online PowerShell에서 다음 cmdlet을 실행합니다.

PowerShellCopy

```
    Set-MailboxAutoReplyConfiguration
```

이 cmdlet에 대한 자세한 내용은 [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration)을 참조하세요.
