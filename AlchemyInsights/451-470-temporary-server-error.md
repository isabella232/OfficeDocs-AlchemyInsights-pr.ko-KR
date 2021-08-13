---
title: 451 4.7.0 임시 서버 오류입니다. 나중에 다시 시도하십시오. PRX4
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2021
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "3000003"
- "12465"
ms.openlocfilehash: ce898981d053c8b5dc080ee83434bdacd7f02a636f0183293915bacdb48ba4ef
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918966"
---
# <a name="451-470-temporary-server-error-please-try-again-later-prx4"></a>451 4.7.0 임시 서버 오류입니다. 나중에 다시 시도하십시오. PRX4

SMTP 클라이언트 전송 방법을 사용하여 Smarthost "smtp.office365.com"를 통해 전자 메일을 보내는 동안 문제가 발생하고 "451 4.7.0 임시 서버 오류입니다. 나중에 다시 시도하십시오. PRX4는 대부분 일시적입니다." 

SMTP 클라이언트 전송 방법을 사용하려면 사용이 허가된 사서함이 필요하기 때문에 SMTP 클라이언트 전송에 공유 사서함을 사용하고 있지 않은지 확인 그러나 공유 사서함을 사용하지 않는 경우 문제가 계속되면 다음을 검사합니다.

1. 다음 PowerShell 명령을 실행하여 사용 중인 사용이 허가된 사서함에서 클라이언트 SMTP 전송을 사용하도록 설정

    ```Set-CASMailbox -Identity sean@contoso.com -SmtpClientAuthenticationDisabled $false```

    또는

    1. 활성 Microsoft 365 관리 센터 > **로 이동하고** 사용자를 선택합니다.
    1. 메일 탭으로 이동 > **전자 메일 >** **앱 관리를 선택합니다.** 
    1. 인증된 **SMTP** 설정이 선택되어 있는지 확인합니다(사용).
    1. **변경 사항 저장** 을 선택합니다.
    
    전체 조직에 대해 SMTP 인증을 사용하도록 설정하려면 다음 명령을 실행합니다.

    `Set-TransportConfig -SmtpClientAuthenticationDisabled $true`
 
    **참고:** 보안상의 이유로 사용되는 사서함에 한해 SMTP 인증을 사용하도록 설정하는 것이 좋습니다. 사용자 수준 설정은 조직 수준 설정에 따라 변경됩니다.

2. 보안 기본값 사용 을 아니요로 전환하여 Azure 보안 **기본값을** 사용하지 **않도록 설정 :**

    1. 보안 관리자, 조건부 액세스 관리자 또는 전역 관리자로 Azure Portal에 로그인합니다.
    1. 속성 Azure Active Directory >**  를 찾아** **보안 기본값 관리를 선택합니다.**
    1. 보안 기본값 **사용 토글을** **아니요로 설정**
    1. **저장** 을 선택합니다.

3. 사용이 허가된 사서함에서 MFA(Multi Factor Authentication)를 사용하지 않도록 설정

    1. 이동하여 Microsoft 365 관리 센터 탐색 메뉴에서 사용자 활성 **사용자를**  >  **선택합니다.**
    1. **활성 사용자** 페이지에서 **다단계 인증** 을 선택합니다.
    1. 사용자를 선택하고 **다단계 인증을 사용하지 않도록 설정합니다.**

