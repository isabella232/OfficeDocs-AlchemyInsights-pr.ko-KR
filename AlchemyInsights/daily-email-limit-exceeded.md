---
title: 일별 전자 메일 제한이 초과 되었습니다. 워크플로가 일시 중단 되었습니다.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 701c4aef6bfc0c4a2c4570f6dd16dbe4f99efc44
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580339"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>일별 전자 메일 제한이 초과 되었습니다. 워크플로가 일시 중단 되었습니다.

이 오류는 다음과 같은 시나리오에서 수신 될 수 있습니다.

- Sharepoint Online의 워크플로를 사용 하 2013 2010 고 있으며,이를 수행 하는 사용자
- 워크플로는 한 번에 200 명 이상의 사용자에 게 사용자 지정 전자 메일 메시지를 전송 하거나, 하루에 1만 명의 받는 사람을 초과 하거나, 분당 30 개 이상의 메시지를 보내도록 구성 됩니다.
- 워크플로를 실행 하면 전자 메일 메시지가 전송 되지 않으며 다음과 같은 동작이 발생 합니다.
    - SharePoint 2013 플랫폼 유형을 사용 하는 워크플로의 경우 **워크플로 상태** 페이지로 이동 합니다. 워크플로 상태 페이지에서 **내부 상태가** **시작**으로 설정 되 고 정보 풍선이 **받는 사람에 게 메시지를 보낼 수 없는**것으로 표시 됩니다.

이 문제를 해결 하려면 [Exchange Online 보낸 사람 제한을](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)초과 하지 않고 전자 메일 메시지를 보내도록 워크플로를 구성 합니다. 예를 들어 워크플로에서 일시 중지를 사용 하거나, Microsoft 365 그룹, 메일 그룹 또는 메일 사용이 가능한 보안 그룹으로 전자 메일을 보내거나, 한 번에 200 명 미만의 받는 사람에 게 메시지를 보냅니다.


자세한 내용은 다음 [문서](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)를 참조 하십시오.

## <a name="related-topics"></a>관련 항목
- [흐름 만들기](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint 및 흐름](https://flow.microsoft.com/blog/sharepoint-and-flow/) 