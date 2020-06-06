---
title: Microsoft 365 앱을 수정 하면 office 라이선스 관련 메시지를 찾을 수 없음
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 65ffae1a784f841cb08a5df52b02671a4526d9d4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580447"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Microsoft 365 앱 "연결 된 office 라이선스를 찾을 수 없음" 메시지를 수정 합니다.

이 메시지가 표시 되 면 다음을 시도해 보세요.

1. 방화벽, 바이러스 백신 소프트웨어 및 프록시 설정을 검사 하 여 Microsoft 365 앱에 대 한 인터넷 액세스를 차단 하 고 있지 않은지 확인 합니다. [Microsoft 365 url 및 IP 주소 범위](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)를 참조 하세요.
2. 영향을 받는 사용자의 Office 라이선스를 제거 하 고 [다시 할당](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) 합니다. 
3. Office 앱을 열고 기존 사용자 계정에서 [로그 아웃](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) 합니다.
4. Windows 설정 > **계정**  >  **전자 메일 & 계정**으로 이동 하 여 영향을 받는 계정을 제외한 모든 작업 계정을 제거 합니다.
5. Windows **설정 >으로**이동 하 여  >  **회사 또는 학교에 액세스**하 고, 영향을 받는 계정을 제외한 모든 작업 계정을 끊으십시오.
6. Office 정품 인증 상태 초기화 [방법을 알아보세요](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. 영향을 받는 사용자 계정을 사용 하 여 [로그인](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) 합니다.

문제 해결 솔루션에 대 한 자세한 내용은 [Office에서 허가 되지 않은 제품 및 정품 인증 오류](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)를 참조 하세요.