---
title: SharePoint 사이트 만들기
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: bf9380727fff415357884a5122e633f2254337d3db50e2b8656d94938f76d394
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080896"
---
# <a name="create-a-sharepoint-site"></a>SharePoint 사이트 만들기

사이트 관리 센터의 [활성](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) 사이트에서 SharePoint 관리합니다. 자세한 내용은 새 사이트 관리 센터에서 [사이트 SharePoint 참조하세요.](https://docs.microsoft.com/sharepoint/manage-site-creation) 

## <a name="tips"></a>팁:

- 기존 **사이트의** URL이 같은 사이트를 만들 수는 없습니다. 사이트를 삭제한 후 URL을 다시 사용하려면 삭제된 사이트가 삭제된 사이트에 계속 존재할 [수 있습니다.](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true) URL을 다시 사용하려면 사이트를 영구적으로 삭제해야 합니다. Powershell을 사용하여 사이트를 완전히 제거하려면 [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet 예제를 참조하세요.
- 일부 사용자는 사이트를 만들 수 없습니다. [Manage site creation in SharePoint Online 를 참조하세요.](https://docs.microsoft.com/sharepoint/manage-site-creation)
- 사이트가 예상보다 길게 만들기에  까다로 표시될 수 있습니다. 이 문제가 처음 확인된 후 24시간 이상이 지난 경우 지원 티켓을 기록하세요. 대부분의 경우 당사는 이미 해결 방법에 대한 작업을 하고 있습니다. 솔루션을 완료하는 데 최소 24시간을 기다렸다가 해결합니다.
