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
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579871"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Microsoft 365 apps "컴퓨터의 신뢰할 수 있는 플랫폼 모듈이 제대로 작동 하지 않습니다." 메시지 수정

이 오류를 해결하려면 다음 단계를 수행하십시오.

- [Windows](https://support.microsoft.com/help/4027667/windows-10-update) 및 [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)용 최신 업데이트를 설치 합니다.
- Windows Credential Manager를 사용 하 여 [Office 자격 증명을 지웁니다](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) .<br/>
    **참고:** Office 2016의 레지스트리 경로가 16.0로 변경 되었습니다. (예: \Software\Microsoft\Office\16.0\Common\Identity\)
- [사용자 복구 프로세스](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) 를 시도 하 여 TPM (신뢰할 수 있는 플랫폼 모듈) 오류를 수정 합니다.
- 다음 단계를 사용 하 여 EnableADAL = 0을 설정 합니다.  
    1. Windows 시작 단추를 마우스 오른쪽 단추로 클릭 하 고 **실행**을 선택한 다음 **regedit**를 입력 하 고 **확인**을 선택 합니다.
    2. 레지스트리 편집기가 장치를 변경할 수 있도록 하려면 **예** 를 선택 합니다.
    3. 레지스트리 편집기에서 HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.에서 설정이 **0** 인 DWORD 값 **EnableADAL** 를 추가 합니다.

자세한 내용은 [Windows 10의 업데이트 후 Office 2016 빌드 16.0.7967에 로그인 후 연결 문제](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)를 참조 하세요.