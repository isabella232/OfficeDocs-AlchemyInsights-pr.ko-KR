---
title: 클래식 루트 사이트를 최신 사이트로 바꾸기
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 7209595f5cda9b31e53241d9d5696fa584ff5e5ab3d237aae28542bf7aec9398
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940825"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>클래식 루트 사이트를 최신 사이트로 바꾸기

2019년 4월 전에 환경을 설정한 경우 Microsoft PowerShell을 사용하여 루트 사이트를 최신 사이트로 변경할 수 있습니다.

- 루트 사이트로 사용할 다른 사이트가 있는 경우 루트 사이트를 [](https://docs.microsoft.com/sharepoint/modern-root-site) 해당 사이트로 대체(스왑)할 수 있습니다. 
    - [Invoke-SPOSiteSwap을](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) 사용하여 원본 사이트를 보관하는 동안 사이트의 위치를 다른 사이트와 바환할 수 있습니다. 팀 사이트(그룹에 연결되지 않은) 및 커뮤니케이션 사이트에 모두 사용할 수 있습니다. 

- 사이트의 콘텐츠를 계속 사용하지만 기존 사이트를 커뮤니케이션 사이트로 변환할 수 있는 추가 기능이 곧 도입될 예정입니다. 
>[!Important]
>이러한 기능은 점진적으로 출시될 것입니다. 메시지 센터에서 업데이트를 계속 확인합니다. 

## <a name="known-issues-with-swapping-sites"></a>사이트 교체와 관련한 알려진 문제

- 대상 사이트에서 짧은 시간 동안 "찾을 수 없습니다"(HTTP 404) 오류가 반환될 수 있습니다.
- 검색 인덱스를 업데이트하려면 콘텐츠를 다시 그려야 합니다. 수동 단계가 필요하지 않습니다. 이 단계는 자동으로 수행됩니다.
- "정적" 링크(예: 파일 동기화 및 OneNote)에 종속된 모든 것을 수동으로 수정해야 합니다.
- 원본 사이트가 조직 뉴스 사이트인 경우 URL을 업데이트합니다. 모든 조직 뉴스 사이트 목록을 얻습니다.
- Project 서버 사이트가 올바르게 연결되도록 서버 사이트의 유효성을 검사해야 할 수 있습니다.
