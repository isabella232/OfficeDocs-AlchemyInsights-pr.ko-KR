---
title: 사이트 그룹에 SharePoint 추가
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
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 5dd159b8b9e141c2fb448bae5fb624efe1014d7d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318130"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>웹 사이트에서 그룹 연결 사이트를 만들 때 SharePoint

1. 그룹 및 연결된 사이트를 삭제하고 동일한 URL로 다른 사이트를 만들 경우 이전 사이트를 영구적으로 제거해야 합니다.

   - [SPO 관리 셸 다운로드](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Powershell 시작에 대한 자세한 내용은 온라인 관리 셸 SharePoint [참조하세요.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)
   - [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet을 사용하여 삭제된 사이트에서 사이트를 제거합니다. 그룹 사이트를 영구적으로 삭제하려면 Powershell이 필요합니다.

1. 그룹 연결 사이트를 만들고 경고가 표시되면 **별칭이** 같은 다른 그룹이 이미 있는 경우 에서 기존 그룹을 [Microsoft 365 관리 센터.](https://admin.microsoft.com/AdminPortal/Home#/groups) 이 문제를 해결하려면 더 이상 필요하지 않은 기존 그룹을 삭제하거나 다른 별칭이 할당된 사이트를 만드면 됩니다.

1. 최신 그룹을 만들고 사용하는 방법에는 여러 가지가 SharePoint.

   - 기존 사이트를 사이트 그룹에 연결할 Microsoft 365 있습니다. 자세한 내용은 커넥트 Microsoft 365 인터페이스를 사용하여 [SharePoint 참조하세요.](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)
   - 그룹 Microsoft 365 사이트를 만들하려면 팀 사이트를 [만들어야 합니다.](https://admin.microsoft.com/sharepoint)
