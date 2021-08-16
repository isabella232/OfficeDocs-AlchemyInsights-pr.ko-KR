---
title: 교육용 고객에 대한 Teams 공통 문제
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
- "9000701"
- "3831"
- "3832"
ms.openlocfilehash: 9dc01109d0f036c567243a8833a845f074097e39de4e1cfc1ba38da61b8f97ab
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049242"
---
# <a name="teams-common-issues-for-education-customers"></a>교육용 고객에 대한 Teams 공통 문제

**교육용 고객의 경우**:

원격 학습을 지원하기 위해 Teams를 배포하는 데 도움이 필요한 경우 [FastTrack 센터](https://www.microsoft.com/fasttrack)를 방문하여 요청을 제출하세요. Teams 교육용 고객에 대한 다음의 공통 문제를 참조하세요.

- **"기회를 놓치고 있습니다."** 메시지가 표시됩니까? [학교에 대한 Microsoft Teams를 사용하도록 설정](https://docs.microsoft.com/microsoft-365/education/intune-edu-trial/enable-microsoft-teams)해야 합니다. EDU 테넌트에서 Microsoft Teams는 기본적으로 사용하도록 설정되어 있지 않습니다. 먼저 이 기능을 사용하도록 설정해야 합니다.

- **Teams를 처음 사용하시나요?** [Office 365 Education에서 원격 교육 및 학습](https://support.office.com/article/remote-teaching-and-learning-in-office-365-education-f651ccae-7b65-478b-8366-51bb884025c4)을 참조하여 학교 설정, 수업 계획, 가상 모임 및 학생들과 콘텐츠 공유에 대한 최신 지침을 알아보세요.

- 이 기능이 설정되면 사용자가 [데스크톱](https://docs.microsoft.com/MicrosoftTeams/get-clients#desktop-client) 또는 [모바일 클라이언트](https://docs.microsoft.com/MicrosoftTeams/get-clients#mobile-clients)를 설치하거나 브라우저(https://teams.microsoft.com)에서 Teams를 실행할 수 있습니다.

- **Teams 게스트 액세스 사용**: [Teams 게스트 액세스 검사 목록](https://docs.microsoft.com/microsoftteams/guest-access-checklist)을 검토하고 모든 단계를 완료했는지 확인합니다.
    - [Microsoft Teams에서 게스트 액세스 이해](https://docs.microsoft.com/microsoftteams/guest-access)
    - [설정 – Microsoft Teams 게스트 액세스 검사 목록](https://docs.microsoft.com/microsoftteams/guest-access-checklist)
    - [게스트가 팀에 참여하는 방법](https://docs.microsoft.com/microsoftteams/guest-joins)

- **Teams 모임 및 전화 접속**: Microsoft Teams에서 오디오 회의를 켜거나 설정하는 데 도움이 필요한가요? 이 사용자가 최근 작성되었나요? 그렇다면 설정을 적용하는 데 2~24시간 기다려야 합니다. 사용자에게 오디오 회의를 사용할 수 있는 라이선스가 부여되었는지와 기본 유료 전화 번호가 있는지 확인하려면 다음을 수행합니다.
    1. 활성 사용자로 이동하고 해당 사용자를 선택합니다.
    2. 관리 센터 버전에 따라, **라이선스 및 앱** 을 선택하거나 **제품 라이선스** 에서 **편집** 을 클릭합니다.
    3. 사용자에게 오디오 회의, Microsoft Teams 및 비즈니스용 Skype(플랜 2)를 사용할 수 있도록 선택된 라이선스가 있는지 확인합니다.
    4. 사용자 관리 센터에서 **모두 표시** 를 클릭한 다음 **Teams** 를 클릭합니다.
    5. Microsoft Teams 관리 센터에서 **레거시 포털** 을 클릭합니다.
    6. 비즈니스용 Skype 관리 센터에서 **오디오 회의** 를 클릭한 다음, **사용자** 를 클릭합니다.
    7. 해당 사용자를 선택하고 사용자에게 기본 유료 전화 번호가 있는지 확인합니다.

    자세한 내용은 [Microsoft Teams 통화 플랜](https://docs.microsoft.com/microsoftteams/calling-plans-for-office-365)을 참조하세요. 라이선스 관련 질문에 대한 도움말을 보려면 Microsoft 상거래 청구 팀에 문의하세요.

    추가 리소스

    - [Microsoft Teams에서의 모임 및 회의](https://docs.microsoft.com/microsoftteams/deploy-meetings-microsoft-teams-landing-page)
    - [오디오 회의](https://docs.microsoft.com/microsoftteams/audio-conferencing-in-office-365)

- **모임 정책**: 모임 정책은 조직에서 사용자가 예약한 모임 참가자가 사용할 수 있는 기능을 제어하는 데 사용됩니다. 정책을 만들고 변경하고 사용자를 정책에 할당할 수 있습니다.

    - **모임 정책 변경 또는 만들기**: 모임 정책을 변경하거나 만들려면 **Microsoft Teams 관리 센터 > 모임 > 모임 정책** 으로 이동합니다. 목록에서 정책을 선택하거나 **추가** 를 클릭합니다. 새 정책을 만들려면 이름과 설명을 추가합니다. 이름은 특수 문자가 포함될 수 없으며 64자를 초과할 수 없습니다. 설정을 선택한 다음 **저장** 을 클릭합니다. 
    
        예를 들어, 사용자 수가 많은데 모임에 필요한 대역폭을 제한하려고 한다고 가정해 보겠습니다. "제한된 대역폭"이라는 새 사용자 지정 정책을 만들고 다음 설정을 사용하지 않도록 설정합니다.

        **오디오 및 비디오** 에서:
        - **클라우드 녹음/녹화 허용** 을 끕니다.
        - **IP 비디오 허용** 을 끕니다.

        **콘텐츠 공유** 에서:

        - 화면 공유 모드를 사용하지 않도록 설정합니다.
        - **화이트보드 허용** 을 끕니다.
        - **공유 노트 허용** 을 끕니다.

        그 다음 **사용자에게 정책을 할당** 합니다.

    1. Microsoft Teams 관리 센터의 왼쪽 탐색 창에서 **사용자** 로 이동한 후 해당 사용자를 클릭합니다.
    2. 사용자 이름의 왼쪽을 클릭하여 사용자를 선택한 후 **설정 편집** 을 클릭합니다.
    3. **모임 정책** 에서 할당하려는 정책을 선택하고 **적용** 을 클릭합니다.

    한 번에 여러 사용자에게 정책을 할당하려면 [Teams 사용자 설정을 일괄 편집](https://docs.microsoft.com/microsoftteams/edit-user-settings-in-bulk)을 참조하세요.

    또는 다음 작업을 수행할 수 있습니다.
    1. Microsoft Teams 관리 센터의 왼쪽 탐색 창에서 **모임 > 모임 정책** 으로 이동합니다.
    2. 정책 이름의 왼쪽을 클릭하여 정책을 선택합니다.
    3. **사용자 관리** 를 클릭합니다.
    4. **사용자 관리** 창에서 표시 이름 또는 사용자 이름으로 사용자를 검색하고 이름을 선택한 후 **추가** 를 클릭합니다. 추가할 각 사용자에 대해 이 단계를 반복합니다.
    5. 사용자 추가를 마쳤으면 **저장** 을 클릭합니다.

- **누락된 다이얼 패드 문제 해결**:
    - 사용자에게 [Teams 라이선스](https://docs.microsoft.com/MicrosoftTeams/assign-teams-licenses)가 할당되어 있는지 확인합니다.
    - 사용자에게 [통화 요금제](https://docs.microsoft.com/MicrosoftTeams/calling-plan-landing-page)가 할당되었는지 확인합니다.
    - 사용자가 [Enterprise Voice](https://docs.microsoft.com/skypeforbusiness/skype-for-business-hybrid-solutions/plan-your-phone-system-cloud-pbx-solution/enable-users-for-enterprise-voice-online-and-phone-system-voicemail#to-enable-your-users-for-phone-system-in-office-365-voice-and-voicemail)를 사용할 수 있도록 설정합니다.

- **Teams 로그인 문제 해결**: 먼저 [Microsoft Teams 서비스가 정상](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/servicehealth)인지 확인합니다. 그런 다음, 자주 발생하는 오류 코드를 확인하고 [Microsoft Teams에 로그인하는 데 문제가 있는 이유](https://support.office.com/article/a02f683b-61a3-4008-9447-ee60c5593b0f)를 검토하세요. [Microsoft Teams의 ID 모델 및 인증](https://docs.microsoft.com/MicrosoftTeams/identify-models-authentication)을 검토해야 할 수도 있습니다.
