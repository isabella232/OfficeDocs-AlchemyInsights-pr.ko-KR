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
- "2556"
ms.openlocfilehash: 7a8a0b68fc211e99b22e857d51d1de54e53a69357f75a0c60b1e83078cd5b27f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088042"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>앱의 빈 Microsoft 365 화면

이 문제를 해결하려는 경우 다음을 시도합니다.
- 에 대한 최신 업데이트를 [Windows](https://support.microsoft.com/help/4027667/windows-10-update) [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- 사용자 Internet Explorer 다시 설정: 도구 인터넷 옵션 고급 초기화 Internet Explorer 설정(사용자 지정 설정이 손실됩니다)로 이동한 다음 다시 Office  >    >    >   합니다.
- WDAG(Windows Defender Application Guard) 또는 유사한 방화벽 또는 바이러스 백신 프로그램을 사용하지 않도록 설정:
    1. 제어판에서 프로그램으로 이동한 다음 기능 Windows **켜기 또는 끄기 를 선택 합니다.**
    2. 이 Windows Defender Application Guard 사용하도록 설정되어 있는 경우 이 기능을 사용 안 하게 합니다.<br/>
    **참고:** 컴퓨터를 다시 시작해야 할 수 있습니다.
- Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) 플러그 인이 응용 프로그램 또는 방화벽/바이러스 백신 프로그램에 의해 차단되지 않는지 확인
- [자격 Office 관리자를 사용하여](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windows 선택을 취소합니다.<br/>
    **참고:** 2016의 레지스트리 Office 16.0으로 변경했습니다. (예: \Software\Microsoft\Office\16.0\Common\Identity\)

자세한 내용은 에서 Office [2016 빌드 16.0.7967로](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)업데이트한 후 로그인 시 연결 문제를 Windows 10.