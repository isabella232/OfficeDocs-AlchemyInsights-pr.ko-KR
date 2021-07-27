---
title: Microsoft 365 메일 서비스에 대한 SMTP 설정
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12073"
- "3000003"
ms.openlocfilehash: 261695a0bf736a51514df50c0ad66aaab5b50edb
ms.sourcegitcommit: e9fcd72e64d35f5ba14dfa0fbde39eae20d86cfe
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/27/2021
ms.locfileid: "53603298"
---
# <a name="smtp-settings-for-the-microsoft-365-mail-service"></a>Microsoft 365 메일 서비스에 대한 SMTP 설정

다음은 Microsoft 365 메일 서비스에 대한 SMTP 설정입니다.

**서버**: smtp.office365.com </br>
**포트**: 587 </br>
**암호화**: STARTTLS(현재 TLS 1.2 버전만 지원됩니다. 응용 프로그램 또는 장치가 TLS 1.2를 지원하는지 확인하세요.) </br>
**사용자 이름**: Office 365 주소(예: example@yourdomain.com) </br>
**암호**: Office 365 암호 </br>
**인증**: 필수 </br>
**전송 한도**: 하루 이메일 10,000통 </br>

POP 및 IMAP 설정은 [POP, IMAP 및 SMTP 설정](https://support.microsoft.com/office/pop-imap-and-smtp-settings-8361e398-8af4-4e97-b147-6c6c4ac95353)을 참조하세요.
 
Microsoft 365를 사용하여 이메일을 릴레이하는 옵션과 단계에 대해 알아보려면 [Microsoft 365 또는 Office 365를 사용하여 이메일을 보내도록 복합기 또는 애플리케이션을 설정하는 방법](/exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365)을 참조하세요.