---
title: 조건부 액세스 문제
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013979"
---
# <a name="conditional-access-issues"></a>조건부 액세스 문제

**로그인 진단 문제 해결**

로그인 진단을 사용하여 발생된 문제를 빠르게 찾거나 사용자 로그인과 관련된 문제를 [진단할 수 있습니다.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. 로그인 진단을 실행합니다.
1. 사용자, 응용 프로그램, 로그인 시간, 요청 ID 또는 상관 관계 ID에 대한 세부 정보를 입력하여 분석할 이벤트를 찾을 수 있습니다.
1. 수행된 작업 및 변경을 위해 수행할 수 있는 작업(변경이 필요한 경우)에 대한 세부 정보를 표시하는 진단 결과를 검토합니다.

**로그인 문제 해결 단계** 

1. Azure AD 로그인 페이지로 이동합니다.
1. 사용자, 시간 범위, 응용 프로그램, 상태, 클라이언트 앱 등으로 로그인을 필터링합니다.
1. 로그인 이벤트를 선택하고 조건부 액세스 탭을 보고 평가된 정책을 볼 수 있습니다.
1. 정책의 행을 클릭하여 정책 세부 정보를 보고 정책이 적용된 이유를 이해합니다.

**조건부 액세스 정책 문제 해결 도구**

- 보고서 전용 모드를 사용하면 사용자에게 영향을 주지 않고 정책을 평가할 수 있습니다.
- 가상 도구를 사용하면 로그인 이벤트를 시뮬레이트하고 적용되는 정책을 볼 수 있습니다.
- 인사이트 및 보고 통합 문서는 각 정책에 대한 실시간 영향을 표시됩니다.

**기준 보호 정책**

기준 보호 정책은 사용되지 않습니다. 더 이상 적용되지는 않습니다. Azure Portal에서 곧 제거됩니다. 보안 기본값을 [사용하도록 설정하는 것이 좋습니다.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)

조건부 액세스에 대한 자세한 내용은 다음을 참조하세요.

[Azure Active Directory의](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 조건부 액세스 모범 사례  
 [조건부 액세스 조건](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [조건부 액세스의 컨트롤](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [조건부 액세스의 위치](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
