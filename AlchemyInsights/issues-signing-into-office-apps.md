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
- "2559"
ms.openlocfilehash: b0789a54f48b2850c1dad8651a8209449c805784bea96799f05e67c4bc43fdb0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986897"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>앱 Microsoft 365 "컴퓨터의 신뢰할 수 있는 플랫폼 모듈이 제대로 작동하지 않습니다." 메시지 수정

이 오류를 해결하려면 다음 단계를 수행하십시오.

- 에 대한 최신 업데이트를 [Windows](https://support.microsoft.com/help/4027667/windows-10-update) [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [자격 Office 관리자를 사용하여](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) Windows 선택을 취소합니다.<br/>
    **참고:** 2016의 레지스트리 Office 16.0으로 변경했습니다. (예: \Software\Microsoft\Office\16.0\Common\Identity\)
- 사용자 [복구 프로세스를 시도하여](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) TPM(신뢰할 수 있는 플랫폼 모듈) 오류를 해결합니다.
- 다음 단계를 사용하여 EnableADAL = 0을 설정하십시오.  
    1. 시작 Windows 마우스 오른쪽 단추를 클릭하고 **실행을** 선택하고 **regedit를** 입력한 다음 확인 을 **선택합니다.**
    2. 레지스트리 **편집기에서** 장치를 변경할 수 있도록 허용하려면 예를 선택합니다.
    3. 레지스트리 편집기에서 설정값이 **0인** **EnableADAL의** DWORD 값을 HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

자세한 내용은 에서 Office [2016 빌드 16.0.7967로](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)업데이트한 후 로그인 시 연결 문제를 Windows 10.