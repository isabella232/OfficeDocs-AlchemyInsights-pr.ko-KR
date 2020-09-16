---
title: SharePoint 사이트에 그룹 추가
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771213"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>SharePoint에서 그룹 연결 된 사이트를 만들 때의 문제

1. 그룹에 연결 된 사이트를 만들거나 다시 만들 때 몇 가지 일반적인 문제가 발생 했습니다.
그룹 및 연결 된 사이트를 삭제 하 고 동일한 URL을 사용 하 여 다른 사이트를 만들려는 경우에는 이전 사이트를 영구적으로 제거 해야 합니다.

   - [SPO 관리 셸](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429) 다운로드
   - Powershell을 시작 하는 방법에 대 한 자세한 내용은 [SharePoint Online 관리 셸을 시작](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)하기를 참조 하세요.
   - [Remove-spodeletedsite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet을 사용 하 여 삭제 된 사이트에서 사이트를 제거 합니다. 그룹 사이트를 영구적으로 삭제 하려면 Powershell이 필요 합니다.

1. 그룹 연결 사이트를 만들고 경고 메시지가 표시 되 면 **다른 그룹의 별칭이 이미**있는 경우 [Microsoft 365 관리 센터](https://admin.microsoft.com/AdminPortal/Home#/groups)에서 기존 그룹을 확인 합니다. 이 문제를 해결 하려면 기존 그룹이 더 이상 필요 하지 않은 경우 삭제 하거나 다른 별칭을 할당 하 여 사이트를 만듭니다.

1. SharePoint에서 최신 그룹을 만들고 사용 하는 방법에는 여러 가지가 있습니다.

   - 기존 사이트를 Microsoft 365 그룹에 연결할 수 있습니다. 자세한 내용은 [SharePoint 사용자 인터페이스를 사용 하 여 a Microsoft 365 그룹 연결](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)을 참조 하십시오.
   - Microsoft 365 그룹 연결 사이트를 만들려면 [팀 사이트](https://admin.microsoft.com/sharepoint)를 만들어야 합니다.
