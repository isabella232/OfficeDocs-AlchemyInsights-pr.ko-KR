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
ms.openlocfilehash: d05c8f02efc3bb92865880ea4a2338abaf7d70254f0b4bbfb566423e62b391dd
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898802"
---
# <a name="investigate-all-the-users-activities"></a>모든 사용자 활동 조사

이 작업을 하는 방법에는 다음이 있습니다.

1. 다음 작업 중 하나를 수행하십시오.
   - 의 Microsoft 365 규정 준수 센터 솔루션 <https://compliance.microsoft.com> **감사로** \> **이동하십시오.** 또는 감사 페이지로 직접 이동하기 위해 **를** <https://compliance.microsoft.com/auditlogsearch> 사용하세요.
   - 의 Microsoft 365 Defender <https://security.microsoft.com> 포털에서 감사로 **이동 합니다.** 또는 감사 페이지로 직접 이동하기 위해 **를** <https://security.microsoft.com/auditlogsearch> 사용하세요.

    > [!NOTE]
    > 기능을 켜야 하다는 알림이 표시면 진행하여 지금 켜야 합니다. 기능이 켜져 있지 않은 경우 검색 결과에서 이전 날짜의 데이터를 끌어오지 못합니다.

2. 감사 **페이지의 검색** **탭에서** 다음 설정을 구성합니다.
   - **날짜 및 시간 범위:** 시작 및  끝  상자에서 날짜/시간 범위를 선택합니다.
   - **활동:** 특정 활동에 관심이 있는 경우 목록에서 선택합니다. 그렇지 않으면 기본값 모든 활동에 대한 결과 **표시는** 모든 활동을 반환합니다.
   - **사용자:** 모든 사용자에 대한 결과를 반환하거나 하나 이상의 사용자를 입력하기 위해 빈 기본값을 수락합니다.

3. 완료되면 검색을 **클릭합니다.** 활동은 새 감사 **검색** 페이지에 표시됩니다. IP **주소,** 사용자 및 활동 **이름이** 표시됩니다.

4. 결과를 다운로드하려면 **모든** 결과 다운로드 \> **내보내기 를 선택합니다.**

5. 결과에서 활동을 선택하여 세부 정보 플라이아웃을 열 수 있습니다.

자세한 내용은 감사 로그 검색을 참조하여 일반적인 지원 [문제를 조사합니다.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
