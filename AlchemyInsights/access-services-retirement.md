---
title: Access 서비스 사용 중지
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
ms.openlocfilehash: 32da879de230dc0ed99563ad881ab5b2479b8453933a127961a26d619e108ab9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938701"
---
# <a name="access-services-retirement"></a>Access 서비스 사용 중지

원래 MC97576에서 발표한 2017년 3월, 지난 해 동안 계속 연락을 Access Services. 이 프로세스의 다음 단계에서는 원본으로 사용하는 데이터 저장소로 SharePoint Access 웹 데이터베이스를 제거합니다.

**이 영향은 어떻게 영향을 미치나요?**

2019년 6월부터 SharePoint Online에서 새 Access 데이터베이스 만들기를 중지하고 2020년 4월까지 서비스 및 나머지 모든 앱을 종료합니다.

**이 변경에 대비하려면 무엇을 해야 하나요?**

조직의 Access 웹 데이터베이스에 대한 전환 계획을 만드는 것이 권장됩니다. 관리자는 Access SharePoint [스캐너를](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) 사용하여 사이트에서 사용하는 Access 앱의 인벤토리를 얻을 수 있습니다.

Access 웹 데이터베이스 데이터를 마이그레이션하는 방법에는 여러 가지가 있습니다.

- 로컬 Access 데이터베이스로 가져오기(. ACCDB) 또는 Excel 파일입니다.
- 또한 웹 및 모바일 Microsoft PowerApps 위한 코드 없는 비즈니스 솔루션을 만들 수 있는 대체 플랫폼으로 사용할 수도 있습니다.