---
title: 콘텐츠 검색 결과 없음
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816854"
---
# <a name="no-results-from-content-searchexports"></a>콘텐츠 검색/내보내기 결과 없음

콘텐츠 검색/내보내기에서 데이터가 반환되지 않는 문제는 특정 관리자가 설정한 특정 준수 보안 필터로 인해 일부 관리자에게 이를 전달하지 못하기 때문일 수 있습니다.

이 문제를 해결하기 위해 이 문제를 유발할 수 있는 준수 보안 필터가 없는지 확인하십시오.
1. 보안 및 준수 센터 Powershell에 연결
2. 다음 명령줄을 실행합니다.
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organization $org