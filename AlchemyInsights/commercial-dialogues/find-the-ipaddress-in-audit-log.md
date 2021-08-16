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
ms.openlocfilehash: 5b58803719df700290f495cb2d2d6742f072420a2a1d393534ca165bb5a14fbb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54017138"
---
# <a name="find-the-ip-address-in-audit-log"></a>감사 로그에서 IP 주소 찾기

1. 사용자 또는 관리자가 수행한 활동에 해당하는 IP 주소가 감사 로그에 표시됩니다. 클라이언트 정보도 기록됩니다. IP 주소를 식별하는 방법에는 다음이 있습니다.

1. 보안 및 [Office 365 센터로 &.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. 감사 **로그**  >  **[검색 검색을 선택합니다.](https://go.microsoft.com/fwlink/?linkid=2103759)**
    > [!NOTE]
    > 감사를 켜야 하는 알림이 표시된 경우 지금 진행하여 켜야 합니다. 이 기능을 사용하도록 설정하지 않은 경우 검색 결과에서 이전 날짜의 데이터를 끌 수 없습니다.
1. 특정 활동에 관심이 있는 경우 활동 목록에서 해당 활동을 **선택합니다.** 그렇지 않으면 기본적으로 선택한 사용자에 대한 모든 활동이 반환됩니다. 특정 활동은 활동 메뉴에서 선택하지 못하게 될 **수** 있습니다. 그러나 모든 활동에 대한 결과  표시를 선택한 경우(기본 설정) 해당 감사 항목이 반환됩니다.
1. 날짜 범위를 지정하고 사용자 **필드에서** 조사할 사용자의 사용자 이름을 선택합니다.
1. **검색** 을 선택합니다. **결과** 아래에 활동들이 나타납니다. 각 활동에 대한 IP 주소를 볼 수 있습니다.
1. 세부 정보를 확인하려면 활동을 선택한 다음 추가 정보 **를 선택합니다.**

자세한 내용은 Search the Office 365 [audit log to troubleshoot common scenarios 를 참조합니다.](https://go.microsoft.com/fwlink/?linkid=2103944)