---
title: 감사 로그에서 IP 주소 및 클라이언트 식별
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: fcad71bcc5ea6036bc8fa25a9be38caabc4d0889ee01ea86e23065333d5fce0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54014906"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>감사 로그에서 IP 주소 및 클라이언트 식별

사용자 또는 관리자가 Microsoft 365 활동에 해당하는 IP 주소가 감사 로그에 표시됩니다. 클라이언트 정보도 기록됩니다. 이러한 정보를 식별하는 단계는 다음과 같습니다.

1. Microsoft 365 [센터에 로그인합니다.](https://protection.office.com/)

2. 검색 감사 **로그 검색**  >  **페이지로** 이동합니다.

   특정 활동에 관심이 있는 경우 활동 목록에서 해당 **활동을** 선택합니다. 그렇지 않은 경우 선택한 사용자에 대한 모든 활동이 반환됩니다(기본 설정).

   **참고:** 활동 메뉴에서 특정 활동을 사용할 수 없는 **경우도** 있습니다. 그러나 모든 활동에 대한 결과  표시를 선택한 경우(기본 설정) 해당 감사 항목이 반환됩니다.

3. 사용자 필드에 사용자 이름을 **지정하고** 활동에 적합한 날짜 범위를 선택한 다음 검색을 **클릭합니다.**

결과 창에서 해당 활동에 대한 IP 주소를 볼 수 있습니다. 감사 레코드를 선택하여 세부 정보  플라이아웃에서 자세한 정보(예: 클라이언트, 작업을 수행한 사용자 등)를 볼 수 있습니다.

자세한 내용은 손상된 계정에 액세스하는 데 사용되는 컴퓨터의 IP 주소 [찾기를 참조하세요.](/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)
