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
ms.openlocfilehash: 565f70d9a09c61bef84cdd1c23e9b0ed34bebe51
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744673"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>앱 Microsoft 365 "죄송합니다. 일시적인 서버 문제가 있습니다." 메시지 수정

참고: 이전 버전의 Windows(예: Windows 7 SP1, Windows Server 2008 R2)를 사용하는 경우 간단한 [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) 수정을 사용하여 TLS 1.2를 기본값으로 사용하도록 설정하십시오. 자세한 내용은 [Windows의 WinHTTP에서 기본 보안 프로토콜로 TLS 1.1 및 TLS 1.2를 사용하도록 업데이트](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)를 참조하세요.

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