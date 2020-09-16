---
title: SharePoint에서 사이트를 영구적으로 삭제
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: bde31f9b197118467ed96d665a9c8edf6b789965
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771727"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a>SharePoint에서 사이트를 영구적으로 삭제

삭제된 사이트의 URL을 다시 사용하거나 (사이트를 다시 작성하기 위해) 더 이상 사용하지 않는 사이트를 영구적으로 삭제하려면 새 SharePoint 관리 센터에서 **영구 삭제**를 사용할 수 있습니다. 

1. [새 SharePoint 관리 센터의 삭제된 사이트 페이지](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true)로 이동하고 조직에 대한 관리자 권한이 있는 계정으로 로그인합니다. 

2. 왼쪽 열에서 사이트를 선택합니다. 

3. **영구 삭제**를 클릭합니다. 

**참고**: 그룹 연결 사이트는 새 SharePoint 관리 센터에서 영구적으로 삭제할 수 없습니다. 대신 [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite)를 사용해야 합니다.  

자세한 내용은 [사이트 영구 삭제](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site)를 참조하세요. 
