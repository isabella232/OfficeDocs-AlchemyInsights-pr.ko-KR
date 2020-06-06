---
title: Microsoft 365 앱에 로그인 하는 문제
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: e4f2fea5c2f368ae240614ee1f7bc729338dd75d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579943"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Microsoft 365 앱 문제 해결 "죄송 합니다. 조직의 다른 계정에 이미 로그인 되어 있습니다." 메시지

이 오류를 해결하려면 다음 단계를 수행하십시오.

- Windows 설정을 사용 하 여 영향을 받는 계정을 제외한 모든 작업 계정을 제거 하 여 **회사 또는 학교 액세스**> 합니다.
- Windows Credential Manager를 사용 하 여 [Office 자격 증명을 지웁니다](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) .<br/>
    **참고:** Office 2016의 레지스트리 경로가 16.0로 변경 되었습니다. (예: \Software\Microsoft\Office\16.0\Common\Identity\)
- Office 앱을 열고 **파일**  >  **계정**  >  **로그 아웃**을 선택 합니다. 유효한 라이선스가 있는 사용자 계정을 사용 하 여 로그인 합니다. 자세한 내용은 [Office의 계정](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)을 참조하세요.
- Mac의 경우 [Mac용 Office 2016 앱에 로그인 할 수 없습니다](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)를 참조하세요.

자세한 내용은 [Office에서 "죄송 합니다." 조직의이 컴퓨터에 다른 계정이 이미 로그인 되어](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)있습니다. "를 참조 하세요.