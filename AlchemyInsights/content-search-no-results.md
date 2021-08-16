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
ms.openlocfilehash: b53534dd0666fa64e692910aa6800abab30169a97fbe567c815ce6b948381a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058008"
---
# <a name="no-results-from-content-searchexports"></a>콘텐츠 검색/내보내기 결과 없음

콘텐츠 검색/내보내기에서 데이터가 반환되지 않는 문제는 특정 관리자가 설정한 특정 준수 보안 필터로 인해 일부 관리자에게 이를 전달하지 못하기 때문일 수 있습니다.

이 문제를 해결하기 위해 이 문제를 유발할 수 있는 준수 보안 필터가 없는지 확인하십시오.
1. 커넥트 및 규정 준수 센터 Powershell에 대한 정보 보호
2. 다음 명령줄을 실행합니다.
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organization $org