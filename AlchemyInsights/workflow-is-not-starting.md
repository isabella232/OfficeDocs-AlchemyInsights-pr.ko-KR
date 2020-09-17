---
title: 워크플로가 시작 되지 않음
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794773"
---
# <a name="workflow-is-not-starting"></a>워크플로가 시작 되지 않음

- SharePoint 2010 및 SharePoint 2013 워크플로가 시작 되지 않습니다.

    - 워크플로가 시작 되지 않는 경우 사용자에 게 워크플로 진행률과 일시적으로 지연이 발생할 수 있는 일시적인 서비스 문제가 있을 수 있습니다. [서비스 상태 대시보드](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) 를 통해 조직에 영향을 준 것이 있는지 확인 합니다.

    - 이 문제가 처음 발생 한 것으로 24 시간 이상 경과 된 경우 지원 티켓을 기록 하세요. 대부분의 경우 당사는 이미 해결 방법에 대한 작업을 하고 있습니다. 솔루션을 완료 하려면 최소한 24 시간 이상 기다려 주세요.

- SharePoint 2010 시작 시 지연 된 워크플로

    - 워크플로가 대규모 일괄 처리에서 트리거되면 발생 합니다. (예: 여러 항목을 한 번에 추가 하는 경우)

    - 워크플로는 실시간으로 실행 되도록 설계 되지 않으므로 지연은 디자인 동작이 됩니다.

   -  워크플로가 복잡 한 XMOL (Extensible Object Markup Language) 인 경우 컴파일이 느려질 수 있습니다. [이](https://support.microsoft.com//kb/3043697) 문서를 확인 하세요.

    - Microsoft SharePoint 2013 워크플로 플랫폼 유형을 사용 하 여 워크플로를 단순화 하거나 다시 디자인 해야 합니다.

    - 워크플로 기록이 커지면 항목을 제거 하거나 새 기록 목록을 만들 수 있습니다.

        자세한 내용은 [워크플로 기록 삭제](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/) 를


## <a name="related-topics"></a>관련 항목
SharePoint Online에서 Microsoft Flow를 시도 하 고 싶으십니까?
- [흐름 만들기](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint 및 흐름](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


