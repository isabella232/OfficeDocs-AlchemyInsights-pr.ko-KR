---
title: 정품 인증 문제-지금은 연결할 수 없습니다.
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725989"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Microsoft 365 앱 "지금 연결 하지 못했습니다." 메시지 수정

이 메시지가 표시 되 면 다음을 시도해 보세요.

1. 방화벽, 바이러스 백신 소프트웨어 및 프록시 설정을 검사 하 여 Microsoft 365 앱에 대 한 인터넷 액세스를 차단 하 고 있지 않은지 확인 합니다. [Microsoft url 및 IP 주소 범위](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)를 참조 하세요.

2. 실행 **시작**으로 이동한  >  **Run**다음 services.msc를 입력 **합니다.** 다음 서비스가 모두 실행 중인지 확인 합니다.
    - 네트워크 연결 장치 자동 설정
    - 네트워크 목록 서비스
    - 네트워크 위치 인식
    - Windows 이벤트 로그

이러한 서비스 중 하나가 실행 되 고 있지 않으면 시작 해 봅니다. 서비스를 시작 하는 데 문제가 있는 경우 상승 된 권한으로 명령 프롬프트를 열어 다음 명령을 실행 합니다.

**sfc/scannow**

이 명령이 완료 되 면 컴퓨터를 다시 시작 합니다.

자세한 내용은 ["미안 하지만 사용자의 계정에 연결할 수 없습니다."를 참조 하세요. 나중에 다시 시도 하세요 (Microsoft 365에서 Office를 정품 인증 하는 경우 오류 발생)](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).