---
title: 루트 사이트로 최신 사이트
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: b42cf276a76547584c8cfd87b5a28f31d51ea7f8ca56621b22aeef01e4613ce6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000398"
---
# <a name="modern-site-as-root-site"></a>루트 사이트로 최신 사이트

클래식 사이트 루트 사이트를 최신 사이트로 교체할 수 있는 새로운 기능을 [출시하기 시작했습니다.](https://docs.microsoft.com/sharepoint/modern-root-site) [Invoke-SPOSiteSwap을](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) 사용하여 원본 사이트를 보관하는 동안 사이트의 위치를 다른 사이트와 바환할 수 있습니다. 팀 사이트(그룹에 연결되지 않은) 및 커뮤니케이션 사이트에 모두 사용할 수 있습니다.

>[!Important]
> 최신 커뮤니케이션 사이트를 만들 수 있도록 클래식 루트 사이트를 삭제하지 않습니다. 이는 Microsoft에서 지원되지 않습니다. 루트 사이트를 삭제하면 사이트를 복원하거나 동일한 URL에 새 사이트를 만들 때까지 조직의 모든 SharePoint 사이트에 액세스할 수 없습니다. 메시지 센터를 통해 이 기능을 전달할 예정입니다. 테넌트에서 기능이 곧 켜져 있을 것으로 예상됩니다.

## <a name="known-issues-with-swapping-sites"></a>사이트 교체와 관련한 알려진 문제
- 대상 사이트에서 짧은 시간 동안 "찾을 수 없습니다"(HTTP 404) 오류가 반환될 수 있습니다.
- 검색 인덱스를 업데이트하려면 콘텐츠를 다시 그려야 합니다. 여기서는 수동 단계가 필요하지 않습니다. 이 단계는 자동으로 수행됩니다.
- "정적" 링크(예: 파일 동기화 및 OneNote)에 종속된 모든 것을 수동으로 수정해야 합니다.
- Project 서버 사이트가 올바르게 연결되도록 서버 사이트의 유효성을 검사해야 할 수 있습니다. 
