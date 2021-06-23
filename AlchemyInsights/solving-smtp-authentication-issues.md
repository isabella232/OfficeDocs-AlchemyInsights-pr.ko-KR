---
title: SMTP 인증 활성화 및 문제 해결
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077657"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>SMTP 인증 활성화 및 문제 해결

사서함에 대해 SMTP 인증을 사용하도록 설정하거나 Microsoft 365 장치 또는 응용 프로그램을 인증하여 전자 메일을 릴레이하려고 할 때 코드 5.7.57 또는 5.7.3 또는 5.7.139와 함께 "클라이언트가 인증되지 않음", "인증 실패" 또는 "SmtpClientAuthentication" 오류가 발생하는 경우 다음 세 가지 작업을 수행하여 문제를 해결하세요.

1. **보안 기본값 사용** 을 **아니요** 로 전환하여 [Azure 보안 기본값](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)을 비활성화합니다.

    a. Azure 포털에 보안 관리자, 조건부 액세스 관리자 또는 전역 관리자로 로그인합니다.<BR/>
    b. Azure Active Directory>  **속성** 으로 이동합니다.<BR/>
    c. **보안 기본값 관리** 를 선택합니다.<BR/>
    d. **보안 기본값 사용** 을 **아니요** 로 설정합니다.<BR/>
    e. **저장** 을 선택합니다.

2. 라이선스가 있는 사서함에서 [클라이언트 SMTP 제출을 사용하도록 설정](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes)합니다.

    a. Microsoft 365 관리 센터에서 **활성 사용자** 로 이동하여 사용자를 선택합니다.<BR/>
    b. 메일 탭으로 이동하고 **이메일 앱** 에서 **이메일 앱 관리** 를 선택합니다.<BR/>
    d. **인증된 SMTP** 이(가) 선택(사용 설정)되었는지 확인합니다.<BR/>
    e. **변경 사항 저장** 을 선택합니다.<BR/>

3. 라이선스가 부여된 사서함에서 [MFA(다단계 인증)를 비활성화](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa)합니다.

    a. Microsoft 365 관리 센터로 이동하고 왼쪽 탐색 메뉴에서 **사용자** > **활성 사용자** 를 선택합니다.<BR/>
    b. **다단계 인증** 을 선택합니다.<BR/>
    c. 사용자를 선택하고 **다단계 인증** 을 비활성화합니다.<BR/>
