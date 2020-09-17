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
ms.openlocfilehash: 5ebaa342ca9864bc31a9ef26eebcf42d96523871
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806945"
---
# <a name="create-a-sharepoint-site"></a>SharePoint 사이트 만들기

SharePoint 관리 센터의 [활성 사이트](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) 에서 사이트를 만들거나 관리 합니다. 자세한 내용은 [새 SharePoint 관리 센터에서 사이트 관리](https://docs.microsoft.com/sharepoint/manage-site-creation)를 참조 하세요. 

## <a name="tips"></a>정보

- 기존 사이트와 동일한 URL을 사용 하 여 사이트를 만들 **수는 없습니다** . 사이트를 삭제 하 고 해당 URL을 다시 사용 하려는 [경우 삭제 된 사이트 아래에](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true)해당 사이트가 계속 남아 있을 수 있습니다. URL을 다시 사용 하려면 사이트를 영구적으로 삭제 해야 합니다. Powershell을 사용 하 여 사이트를 완전히 제거 하려면 [제거-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet 예제를 참조 하세요.
- 일부 사용자가 사이트를 만들지 못할 수 있습니다. [SharePoint Online에서 사이트 만들기 관리를 참조](https://docs.microsoft.com/sharepoint/manage-site-creation)하세요.
- 사이트가 예상 보다 오래 **생성** 되는 것 처럼 표시 될 수 있습니다. 이 문제가 처음 발생 한 것으로 24 시간 이상 경과 된 경우 지원 티켓을 기록 하세요. 대부분의 경우 당사는 이미 해결 방법에 대한 작업을 하고 있습니다. 솔루션을 완료 하려면 최소한 24 시간 이상 기다려 주세요.
