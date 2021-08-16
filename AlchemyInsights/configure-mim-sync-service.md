---
title: MIM 동기화 서비스 구성
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: f834bead0b6f22dcadc808d45dcefe7f6571ef62c74b7fd97355157ca49542af
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53978491"
---
# <a name="configure-mim-sync-service"></a>MIM 동기화 서비스 구성

Microsoft Identity Manager(MIM) 동기화 서비스는 MIM의 구성 요소입니다. 이 서비스는 여러 개의 온-프레미스 디렉터리 및 데이터베이스가 있는 조직의 정보를 저장하고 통합하는 중앙 집중식 온-프레미스 서비스입니다. MIM 최신 업데이트에서 다루어졌거나 아래 섹션에 언급된 다른 문제 중 하나인 MIM 동기화 문제를 해결할 수 있습니다.

**다음 권장 단계**

1. MIM 동기화의 최신 업데이트를 사용하고 있는지 확인하고 [MIM 동기화 릴리스 정보](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history)를 확인하여 업데이트에서 문제가 해결되었는지 알아봅니다.
2. 일반 LDAP, 일반 SQL, Lotus Domino 또는 웹 서비스 커넥터에 문제가 있는 경우 [일반 커넥터](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)의 최신 업데이트를 사용하고 있는지 확인합니다.
3. 오류로 인해 MIM 동기화 실행이 중지되는 경우 [실행 오류 코드](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) 표를 참조하여 가능한 원인을 파악합니다.
4. **extension-dll 예외** 로 실행이 중지된 경우라면 해당 단어를 클릭하여 **커넥터 공간 개체 속성** 창을 열고 **스택 추적...** 을 클릭하여 [Extension-DLL 예외](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx)에 기술된 자세한 근본 원인 정보를 확인합니다.
5. PCNS(암호 변경 알림 서비스) 구성 요소가 암호 동기화 동안 이벤트 로그에 **오류 6025** 를 보고하는 경우, [PCNS 보고 오류 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx)를 해결하는 가이드를 확인합니다.
6. FIM 서비스 관리 에이전트와의 전체 동기화가 느린 경우 TempDB의 **자동 키우기** 설정을 [전체 동기화가 느리거나 중단된 경우 문제 해결](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx)에 기술된 대로 확인합니다.
7. FIM 서비스 관리 에이전트를 사용하여 웹 서비스를 통한 만들기 실패로 중지된 서버 오류가 발생하는 경우 [지원 정보: 웹 서비스를 통한 만들기 실패](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services)의 원인 개요를 참조하세요.

