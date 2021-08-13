---
title: 보관 사서함으로 전자 메일 메시지 이동
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
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 7e72766f441e210a81fcfd6c07b1801f6c0474afb02a70edf2ad8dbb571f3d2a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974963"
---
# <a name="move-email-to-the-archive-mailbox"></a>보관 사서함으로 전자 메일 이동

아래에 언급된 설정에 대한 자동 검사를 실행하려면 이 페이지 맨 위에 있는 뒤로 단추 <-를 선택한 다음 전자 메일을 보관 사서함으로 이동하는 데 문제가 있는 사용자의 전자 메일 주소를 입력합니다.

1. 보관 **사서함이 사용하도록** 설정되어 있는지 확인합니다. 그렇지 않은 경우 이 [](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) 문서의 단계를 사용하여 보관 사서함을 사용하도록 설정할 수 있습니다.

2. 메시지를 보관 사서함에 자동으로 보관하려면 보관 사서함으로 이동 작업이 있는 보존 태그를 전체 사서함(기본값) 태그에 자동으로 적용 으로 **설정해야 합니다.**  다음 단계에 따라 태그를 만들 수 있습니다. [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. 그런 다음 보존 정책에 **보관** 태그를 추가합니다. in the Exchange admin center, choose **Retention Policies** > add the Move to Archive **tag to** the policy > **Save.**

4. 이제 [특정 사용자의 사서함에](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) 보존 정책을 할당합니다. 기본 사서함과 보관 **사서함에** 동일한 **정책이** 적용됩니다.

MFA(관리되는 폴더 도우미)를 강제로 실행하고 사용자 사서함에 새 설정을 적용해야 할 수 있습니다. [EXO PowerShell에](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) 연결된 동안 다음 명령을 실행하여 특정 사서함에 대해 관리되는 폴더 도우미를 시작할 수 있습니다.
  
Start-ManagedFolderAssistant -Identity <name of the mailbox>

보관 정책 설정에 대한 자세한 내용은 사서함에 대한 보관 및 삭제 정책 설정을 [참조하세요.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)
  