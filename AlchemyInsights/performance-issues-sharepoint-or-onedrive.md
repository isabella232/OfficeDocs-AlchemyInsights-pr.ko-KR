---
title: 성능 문제로 SharePoint 또는 OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 921aae7eba8487c5600f290fd671ef2675372e6af0478b913e38354856cbaa22
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911848"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint 또는 OneDrive 사용자에 대해 느리거나, 사용할 수 없거나, 사용할 수 없는 경우

SharePoint OneDrive 속도가 느리거나, 사용할 수 없거나, 사용할 수 없거나, 여러 가지 이유로 인해 서비스를 사용할 수 없거나 503 오류가 표시될 수 있습니다.
  
- 여러 SharePoint 또는 OneDrive 사이트가 느리거나 지연되는 경우 사용자가 SharePoint 사이트 또는 콘텐츠에 액세스할 때 탐색 오류가 일시적으로 발생하는 OneDrive 있습니다. 조직에 영향을 미치는지 확인하려면 [서비스 상태 대시보드](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)를 확인하세요.
  
- 사용자가 사이트 또는 다른 사이트로 이동하려고 할 때 *503* 서버 사용 중 오류가 SharePoint OneDrive 있습니다. 이 오류는 서비스 내의 스로틀로 인해 SharePoint 있습니다. SharePoint Online은 제한된 기능을 사용하여 SharePoint Online 서비스의 최상의 성능과 안정성을 유지합니다. 제한 기능은 사용자 작업 수 또는 동시 호출 수(스크립트 또는 코드에 의한)를 제한하여 리소스가 과도하게 사용되지 않도록 합니다. 스로틀에 대한 자세한 내용은 Online에서 스로틀링 또는 차단되지 [않도록 방지를 SharePoint 참조하세요.](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- 사이트 또는 페이지의 클래식 또는  최신 SharePoint 성능이 저하되는 경우 [](https://aka.ms/perftool) 페이지 진단 도구를 사용하여 페이지를 분석합니다. 
  
- 일반적인 성능 저하가 계속되는 경우 이 문서 아래쪽의 리소스를 검토하세요. [SharePoint Online용](https://go.microsoft.com/fwlink/?linkid=2024334) 성능 조정 소개
  