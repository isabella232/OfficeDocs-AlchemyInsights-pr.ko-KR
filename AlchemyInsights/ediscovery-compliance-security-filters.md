---
title: 콘텐츠 검색/내보내기 중에 결과가 반환되지 않습니다.
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: 8786f11f170edb151879235e19caa38b50f3f06e
ms.sourcegitcommit: 3d662e1a1440ba74b5347896347d03bb8c8f3af5
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/22/2020
ms.locfileid: "49727229"
---
# <a name="no-results-returned-during-content-searchexport"></a>콘텐츠 검색/내보내기 중에 결과가 반환되지 않습니다.

다음과 같은 eDiscovery 시나리오에 문제가 있는 경우

- 콘텐츠 검색/내보내기에서 데이터 또는 예기치 않은 데이터가 반환되지 않습니다.
- eDiscovery 검색 또는 내보내기 실패

특정 관리자가 설정하고 모든 관리자에게 전달되지 않은 특정 준수 보안 필터 때문일 수 있습니다.

이 문제를 해결하기 위해 이러한 문제를 유발할 수 있는 준수 보안 필터가 없는지 확인하십시오.

1. 보안 및 준수 센터 Powershell에 연결
2. 다음 commandlet을 실행합니다.

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

준수 보안 필터에 대한 자세한 내용은 콘텐츠 검색에 대한 사용 권한 [필터링을 참조하세요.](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
