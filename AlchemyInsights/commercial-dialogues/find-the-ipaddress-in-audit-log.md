---
title: 감사 로그에서 IP 주소 찾기
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 258e92368b8a33e8ea807f0cb9af90132c86ed5b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58303583"
---
# <a name="find-the-ip-address-in-audit-log"></a>감사 로그에서 IP 주소 찾기

사용자 또는 관리자가 수행한 활동에 해당하는 IP 주소가 감사 로그에 표시됩니다. 클라이언트 정보도 기록됩니다. IP 주소를 식별하는 방법에는 다음이 있습니다.

1. 다음 작업 중 하나를 수행하십시오.
   - <https://compliance.microsoft.com>의 Microsoft 365 규정 준수 센터에서 **솔루션** \> **감사** 로 이동하세요. 또는 <https://compliance.microsoft.com/auditlogsearch>에서 **감사** 로 직접 이동하세요.
   - <https://security.microsoft.com>의 Microsoft 365 Defender에서 **감사** 로 이동하세요. 또는 <https://security.microsoft.com/auditlogsearch>에서 **감사** 로 직접 이동하세요.

    **참고:** 감사를 켜야 하다는 알림이 표시면 지금 진행하여 켜야 합니다. 이 기능을 사용하도록 설정하지 않은 경우 검색 결과에서 이전 날짜의 데이터를 끌 수 없습니다.

2. **감사** 페이지에서 **검색** 탭이 선택되었는지 확인하고 다음 설정을 구성하세요.
   - **날짜 및 시간 범위**: **시작** 및 **종료** 살자에서 날짜/시간 범위ㄹ르를 선택하세요.
   - **활동:** 특정 활동에 관심이 있는 경우 목록에서 선택합니다. 그렇지 않으면 기본값 모든 활동에 대한 결과 **표시는** 반환되는 모든 활동을 반환합니다. 특정 활동을 선택하지 못하게 될 수 있습니다. 그러나 모든 활동에 대한 결과  표시가 선택된 경우 해당 감사 항목이 반환됩니다.
   - **사용자**: 모든 사용자에 대한 결과를 반환하려면 빈 기본값을 그대로 사용하거나 한 명 이상의 사용자를 입력합니다.

3. 마쳤으면 **검색** 을 클릭합니다. 활동은 새 **검색 감사** 페이지에 표시됩니다.

4. 결과에서 **결과 필터링** 을 클릭하고 활동 필터링 상자에서 **Set-Mailbox** 를 입력하세요.

5. 결과에서 감사 레코드를 선택하여 **세부** 정보 플라이아웃을 열 수 있습니다.

자세한 내용은 감사 로그를 검색하여 일반적인 지원 [문제 조사를 참조하세요.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
