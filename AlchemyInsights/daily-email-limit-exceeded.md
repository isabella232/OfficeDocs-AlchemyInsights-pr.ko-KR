---
title: 일별 전자 메일 제한이 초과됩니다. 워크플로가 일시 중단되었습니다.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 60ddbe68298e998a4e0b271a15209efc135c80638702c98dbcb3e0b2f1554860
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914657"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>일별 전자 메일 제한 초과. 워크플로가 일시 중단되었습니다.

이 오류는 다음과 같은 시나리오에서 수신될 수 있습니다.

- SharePoint 2010 또는 SharePoint 2013 워크플로 플랫폼 유형을 사용하는 워크플로가 SharePoint 있습니다.
- 워크플로는 한에 200명 이상의 사용자에게 사용자 지정 전자 메일 메시지를 보내거나, 하루 10,000명 이상의 받는 사람 또는 분당 30개 이상의 메시지를 보내도록 구성됩니다.
- 워크플로를 실행하면 전자 메일 메시지가 전송되지 않습니다. 다음과 같은 동작이 나타납니다.
    - SharePoint 플랫폼 유형을 사용하는 워크플로의 경우 워크플로 상태 **페이지로** 이동합니다. 워크플로 상태 페이지에서 내부  상태가 시작으로 설정되어 **있으며** 정보 풍선에 받는 사람에게 보낼 수 **없습니다.가 표시됩니다.**

이 문제를 해결하기 위해 보낸 사람 제한을 초과하지 않고 전자 메일 메시지를 보내도록 워크플로를 [Exchange Online 합니다.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits) 예를 들어 워크플로에서 일시 중지를 사용하여 Microsoft 365 그룹, 메일 그룹 또는 메일 사용이 가능한 보안 그룹으로 전자 메일을 보내거나 메시지를 한에 200명 미만의 받는 사람에게 보냅니다.


자세한 내용은 다음 문서를 [참조하세요.](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)

## <a name="related-topics"></a>관련 항목
- [사용자 Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint 및 Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 