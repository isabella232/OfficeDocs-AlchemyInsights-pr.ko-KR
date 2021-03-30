---
title: 워크플로가 시작되지 않습니다.
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
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403749"
---
# <a name="workflow-is-not-starting"></a>워크플로가 시작되지 않습니다.

- SharePoint 2010 및 SharePoint 2013 워크플로가 시작되지 않습니다.

    - 워크플로가 시작되지 않는 경우 워크플로 진행률에 따라 사용자에게 일시적인 지연이 생략될 수 있는 임시 서비스 문제가 있을 수 있습니다. 서비스 상태 [대시보드를](https://admin.microsoft.com/AdminPortal/Home/servicehealth) 확인하여 조직에 영향을 미치는지 확인할 수 있습니다.

    - 이 문제가 처음 확인된 후 24시간 이상이 지난 경우 지원 티켓을 기록하세요. 대부분의 경우 당사는 이미 해결 방법에 대한 작업을 하고 있습니다. 솔루션을 완료하는 데 최소 24시간을 기다렸다가 해결합니다.

- 시작 시 SharePoint 2010 워크플로가 지연됩니다.

    - 워크플로가 대규모 일괄 처리에서 트리거되는 경우 발생합니다. 예를 들어 한에 여러 항목이 추가된 경우입니다.

    - 워크플로는 실시간으로 실행하도록 설계되지 않은 것이기 때문에 지연은 디자인된 동작입니다.

   -  워크플로가 XMOL(Extensible Object Markup Language)이 복잡하면 컴파일 속도가 느려질 수 있습니다. 이 [문서를 확인](https://support.microsoft.com//kb/3043697) 합니다.

    - Microsoft SharePoint 2013 워크플로 플랫폼 유형을 사용하여 워크플로를 단순화하거나 다시 디자인해야 합니다.

    - 워크플로 기록이 커진 경우 항목을 제거하거나 새 기록 목록을 만들 수 있습니다.

        추가 정보: [워크플로 기록 제거](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>관련 항목
SharePoint Online에서 Microsoft Flow를 사용해 보시겠습니까?
- [흐름 만들기](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint 및 Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
