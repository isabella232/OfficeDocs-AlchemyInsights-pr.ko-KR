---
title: 모든 사용자 활동 조사
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 016f4b1caa05cb26d1e6795551b64737d4cb64a5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332349"
---
# <a name="investigate-all-the-users-activities"></a>모든 사용자 활동 조사

이 작업을 하는 방법에는 다음이 있습니다.

1. 다음 작업 중 하나를 수행하십시오.
   - <https://compliance.microsoft.com>의 Microsoft 365 규정 준수 센터에서 **솔루션** \> **감사** 로 이동하세요. 또는 <https://compliance.microsoft.com/auditlogsearch>에서 **감사** 로 직접 이동하세요.
   - <https://security.microsoft.com>의 Microsoft 365 Defender에서 **감사** 로 이동하세요. 또는 <https://security.microsoft.com/auditlogsearch>에서 **감사** 로 직접 이동하세요.

    **참고:** 기능을 켜야 하다는 알림이 표시된 경우 앞으로 이동하여 지금 켜야 합니다. 기능이 켜져 있지 않은 경우 검색 결과에서 이전 날짜의 데이터를 끌어오지 못합니다.

2. 감사 **페이지의 검색** **탭에서** 다음 설정을 구성합니다.
   - **날짜 및 시간 범위**: **시작** 및 **종료** 살자에서 날짜/시간 범위ㄹ르를 선택하세요.
   - **활동:** 특정 활동에 관심이 있는 경우 목록에서 선택합니다. 그렇지 않으면 기본값 모든 활동에 대한 결과 **표시는** 모든 활동을 반환합니다.
   - **사용자**: 모든 사용자에 대한 결과를 반환하려면 빈 기본값을 그대로 사용하거나 한 명 이상의 사용자를 입력합니다.

3. 마쳤으면 **검색** 을 클릭합니다. 활동은 새 **검색 감사** 페이지에 표시됩니다. IP **주소,** 사용자 및 활동 **이름이** 표시됩니다.

4. 결과를 다운로드하려면 **모든** 결과 다운로드 \> **내보내기 를 선택합니다.**

5. 결과에서 활동을 선택하여 세부 정보 플라이아웃을 열 수 있습니다.

자세한 내용은 감사 로그 검색을 참조하여 일반적인 지원 [문제를 조사합니다.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
