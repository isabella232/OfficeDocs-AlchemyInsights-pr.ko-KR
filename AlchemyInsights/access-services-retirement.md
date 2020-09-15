---
title: Access services 퇴직
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698688"
---
# <a name="access-services-retirement"></a>Access services 퇴직

처음에 발표 된 것 처럼, 3 월 2017 일에 MC97576, 지난 해 액세스 서비스를 통한 통신은 곧 사용 중지 되었습니다. 이 프로세스의 다음 단계는 SharePoint 목록을 기본 데이터 저장소로 사용 하는 Access 웹 데이터베이스를 제거 하는 것입니다.

**어떤 영향을 줍니까?**

2019 년 6 월부터 시작 하 여 SharePoint Online에서 새 Access 데이터베이스 만들기를 중지 하 고 서비스 및 나머지 모든 앱을 4 월 2020까지 종료 합니다.

**이 변경 사항을 준비 하려면 어떻게 해야 하나요?**

조직의 Access 웹 데이터베이스에 대 한 전환 계획을 만드는 것이 좋습니다. 관리자는 [SharePoint access 앱 검색](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) 프로그램을 사용 하 여 사이트에서 사용 중인 Access 앱의 인벤토리를 가져올 수 있습니다.

Access 웹 데이터베이스 데이터를 마이그레이션하는 방법에는 여러 가지가 있습니다.

- 로컬 Access 데이터베이스 (. ACCDB) 또는 Excel 파일에 추가할 수 있습니다.
- 또한 웹 및 모바일 장치용 코드 없는 비즈니스 솔루션을 만드는 대체 플랫폼으로 Microsoft PowerApps를 탐색 하는 것이 좋습니다.