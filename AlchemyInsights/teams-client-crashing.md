---
title: Teams 클라이언트의 작동이 중지되나요?
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
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826277"
---
# <a name="teams-client-crashing"></a>Teams 클라이언트의 작동이 중지되나요?

Teams 클라이언트의 작동이 중단되면 다음을 시도해 보세요.

- Teams 데스크톱 앱을 사용하는 경우 [앱이 완전히 업데이트되었는지 확인합니다](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- 모든 [Microsoft 365 URL 및 주소 범위](https://docs.microsoft.com/microsoftteams/connectivity-issues)에 액세스할 수 있는지 확인합니다.

- 테넌트 관리자 계정으로 로그인하고 [서비스 상태 대시보드](https://docs.microsoft.com/office365/enterprise/view-service-health)를 확인하여 작동 중단 또는 서비스 저하가 없는지 확인합니다.

- Teams 애플리케이션 제거 및 다시 설치(링크)
    - 컴퓨터에서 %appdata%\Microsoft\teams\ folder로 이동하고 디렉터리의 모든 파일을 삭제합니다.
    - [Teams 앱을 다운로드 및 설치](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)하고 가능한 경우, 관리자로 Teams를 설치합니다(Teams 설치 관리자를 오른쪽 마우스로 클릭하고 가능한 경우 “관리자로 실행” 선택).

Teams 클라이언트가 계속 충돌하는 경우, 문제를 재현할 수 있나요? 그럴 경우, 다음을 수행합니다.

1. 단계 레코더를 사용하여 단계를 캡처할 수 있습니다.
    - 불필요하거나 중요한 응용 프로그램을 모두 종료합니다.
    - 단계 레코더를 시작하고 영향을 받은 사용자 계정으로 로그인하여 문제를 재현해 보세요.
    - [기록한 재현 단계를 캡처하는 팀 로그를 수집합니다](https://docs.microsoft.com/microsoftteams/log-files). **참고**: 영향을 받은 사용자의 로그인 주소를 캡처해야 합니다.
    - 덤프 및/또는 오류 버킷 정보를 수집합니다(Windows). 충돌이 발생하는 컴퓨터에서 Windows Powershell을 실행하고 다음 명령을 실행합니다.

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. 고객 지원 서비스 케이스에 파일을 첨부합니다.
