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
ms.openlocfilehash: c3b1cac5379f4f3da93152fa20086068f7df562cd98b2980ce1b4280e0aa6d5f
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57902266"
---
# <a name="find-the-ip-address-in-audit-log"></a>감사 로그에서 IP 주소 찾기

사용자 또는 관리자가 수행한 활동에 해당하는 IP 주소가 감사 로그에 표시됩니다. 클라이언트 정보도 기록됩니다. IP 주소를 식별하는 방법에는 다음이 있습니다.

1. 다음 작업 중 하나를 수행하십시오.
   - 의 Microsoft 365 규정 준수 센터 솔루션 <https://compliance.microsoft.com> **감사로** \> **이동하십시오.** 또는 감사 페이지로 직접 이동하기 위해 **를** <https://compliance.microsoft.com/auditlogsearch> 사용하세요.
   - 의 Microsoft 365 Defender <https://security.microsoft.com> 포털에서 감사로 **이동 합니다.** 또는 감사 페이지로 직접 이동하기 위해 **를** <https://security.microsoft.com/auditlogsearch> 사용하세요.

    > [!NOTE]
    > 감사를 켜야 하는 알림이 표시된 경우 지금 진행하여 켜야 합니다. 이 기능을 사용하도록 설정하지 않은 경우 검색 결과에서 이전 날짜의 데이터를 끌 수 없습니다.

2. 감사 **페이지에서** 검색 탭이  선택되어 있는지 확인한 후 다음 설정을 구성합니다.
   - **날짜 및 시간 범위:** 시작 및  끝  상자에서 날짜/시간 범위를 선택합니다.
   - **활동:** 특정 활동에 관심이 있는 경우 목록에서 선택합니다. 그렇지 않으면 기본값 모든 활동에 대한 결과 **표시는** 반환되는 모든 활동을 반환합니다. 특정 활동을 선택하지 못하게 될 수 있습니다. 그러나 모든 활동에 대한 결과  표시가 선택된 경우 해당 감사 항목이 반환됩니다.
   - **사용자:** 모든 사용자에 대한 결과를 반환하거나 하나 이상의 사용자를 입력하기 위해 빈 기본값을 수락합니다.

3. 완료되면 검색을 **클릭합니다.** 활동은 새 감사 **검색** 페이지에 표시됩니다.

4. 결과에서 결과 **필터링을** 클릭하고 활동 필터 상자에 **Set-Mailbox를** 입력합니다.

5. 결과에서 감사 레코드를 선택하여 **세부** 정보 플라이아웃을 열 수 있습니다.

자세한 내용은 감사 로그를 검색하여 일반적인 지원 [문제 조사를 참조하세요.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
