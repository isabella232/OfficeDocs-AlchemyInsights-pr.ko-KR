---
title: 앱 Microsoft 365 수정 죄송합니다. 일시적인 서버 문제 메시지가 있습니다.
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
- "3420"
- "9001430"
ms.openlocfilehash: aa0d625856df1027146de5af57845224e3056d8c21d9ac4cefbd4a9c329f487c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54021602"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>앱 Microsoft 365 "죄송합니다. 일시적인 서버 문제가 있습니다." 메시지 수정

이 메시지를 받으면 다음을 시도해 보아야 합니다.

1. 방화벽, 바이러스 백신 소프트웨어 및 프록시 설정을 확인하여 방화벽이 앱에 대한 인터넷 액세스를 차단하지 Microsoft 365 확인합니다. URL [및 IP 주소 범위를 참조하세요.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. 시작   >  **실행으로 이동한** 다음 **services.msc 를 입력합니다.** 다음 서비스가 모두 실행 중인지 확인
    - 네트워크 연결 장치 자동 설정
    - 네트워크 목록 서비스
    - 네트워크 위치 인식
    - Windows 이벤트 로그

이러한 서비스 중 하나에서 실행되고 있지 않은 경우 시작해 보아야 합니다. 서비스를 시작하는 데 문제가 있는 경우 상승된 사용 권한으로 명령 프롬프트를 열고 다음 명령을 실행합니다.

**sfc /scannow**

이 명령이 완료되면 컴퓨터를 다시 시작합니다.

자세한 내용은 ["죄송합니다. 계정에 연결할 수 없습니다. 나중에 다시 시도하세요" 오류를 활성화하면 오류가 발생합니다.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)