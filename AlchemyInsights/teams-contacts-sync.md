---
title: Teams 연락처 동기화
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
- "9004610"
- "11540"
ms.openlocfilehash: 0ffa91f0e31a4904db87f0df6d9b4c51b05ae2758a5ce0d96c77ef4456f6d033
ms.sourcegitcommit: 71501cde5bcb73f4dcf23944d400a4db10f37033
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/09/2021
ms.locfileid: "57807195"
---
# <a name="teams-contacts-sync"></a>Teams 연락처 동기화

Teams는 조직 Active Directory의 연락처와 사용자의 Outlook 기본 폴더에 추가된 연락처를 사용합니다. 연락처가 Microsoft Teams에 표시되지 않으면 다음을 시도하세요.

**참고:** 하나 이상의 연락처에 대한 정보가 최근에 업데이트된 경우 연락처가 동기화되는 데 최대 48시간이 걸릴 수 있습니다.

1. Teams에서 로그아웃하고 다시 시작합니다. 연락처가 표시되는지 확인합니다.
1. Teams 캐시 지우기:
    1. **%appdata%\Microsoft\Teams** 로 이동합니다.
    1. 폴더의 내용을 삭제합니다.
    1. 컴퓨터를 다시 시작하고 Teams를 시작합니다.
1. 연락처가 Outlook에 있는 경우 연락처 목록에 추가해야 합니다. Outlook의 주소 표시줄에서 **파일** 을 선택한 다음 **연락처에 추가** 를 선택합니다.
1. 사용자의 Exchange 사서함이 (온-프레미스가 아닌) 온라인에 호스팅되어 있는지 확인합니다. 자세한 내용은 [Exchange와 Microsoft Teams의 상호 작용 방식](/microsoftteams/exchange-teams-interact)을 참조하세요.
1. 연락처 정보에 연락처의 전화 번호가 추가되었는지 확인합니다.
1. 검색 표시줄에서 연락처의 전자 메일을 검색합니다. 연락처 목록에 대한 동기화를 재개할 수 있는 연락처입니다.
