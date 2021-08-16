---
title: 앱에 로그인하는 Microsoft 365 문제
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: 454000eafa6818f91e3c302cc69fbf252aae1107aa18904ac93a4756d4db642b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028046"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>앱 Microsoft 365 "죄송합니다. 조직의 다른 계정이 이미 로그인되어 있습니다." 메시지 수정

이 오류를 해결하려면 다음 단계를 수행하십시오.

- 영향을 받는 계정을 제외한 모든 직장 계정을 제거하고 Windows 설정 > 또는 학교 액세스 **를 사용하여 제거합니다.**
- [자격 Office 관리자를 사용하여](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows 선택을 취소합니다.<br/>
    **참고:** 2016의 레지스트리 Office 16.0으로 변경했습니다. (예: \Software\Microsoft\Office\16.0\Common\Identity\)
- 파일 Office 앱 **계정** 로그인  >    >  **을 선택하세요.** 그런 다음 유효한 라이선스가 있는 사용자 계정을 사용하여 로그인합니다. 자세한 내용은 [Office의 계정](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)을 참조하세요.
- Mac의 경우 [Mac용 Office 2016 앱에 로그인 할 수 없습니다](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)를 참조하세요.

자세한 내용은 에서 "죄송합니다. 조직의 다른 계정이 이미 이 [컴퓨터에 로그인되어 있습니다."를 Office.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)