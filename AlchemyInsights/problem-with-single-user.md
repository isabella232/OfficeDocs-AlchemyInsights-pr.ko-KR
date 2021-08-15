---
title: 단일 사용자 문제
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: 8d8821cda94b2af244fa317707421f9d197b6052fb316789cd286ea8b4adf19e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960157"
---
# <a name="problem-with-single-user"></a>단일 사용자 문제

- 서비스에서 아직 사용자를 평가할 기회가 제공되지 않았기 때문에 사용자가 프로비전되지 않았을 수 있습니다. 프로비전에 걸리는 시간 및 프로비저닝 구성 페이지의 진행률 표시줄에 대한 지침을 검토합니다. 추가 세부 정보 섹션에 지정된 상태가 사용자가 생성/업데이트/삭제된 날짜 이전인 경우 아직 사용자를 평가하지 않은 것입니다. 이 시나리오에서 가장 좋은 일은 프로비저닝 서비스가 완료될 때까지 기다리는 것입니다.

  - 이 서비스는 원본 시스템(클라우드 HR)의 사용자에 대한 변경 내용만 인식합니다. Azure AD의 원본 시스템에서 변경을 감지하고 Active Directory로 흐름하기 위해 유효한 변경이 있어야 합니다.
- 프로비저닝 서비스에서 사용자를 평가하고 프로비전하지 않는 것으로 결정했습니다.
  - 특성 기반의 지정 필터를 설정한 경우 사용자가 지정한 조건을 충족하는지 확인
  - 사용자가 대상 시스템에 이미 있으며 원본 및 대상 일치의 사용자 상태가 일치하는 경우 추가 작업을 수행하지 않습니다.
- 프로비저닝 서비스가 사용자를 프로비전하려고 했지만 실패했습니다. 이러한 시나리오의 경우 프로비저닝 로그의 문제 해결 및 권장 사항 탭을 검토합니다.
  - 사용자의 필수 특성이 사내 Active Directory 또는 Azure AD에 누락될 수 있습니다. 예를 들어 userPrincipalName 또는 sAMAccountName 생성 규칙이 올바른 값을 생성하지 않습니다.
  - 일치하는 특성(일반적으로 employeeId)은 사내 Active Directory 또는 Azure AD의 고유 사용자에게는 해당되지 않습니다. 예를 들어 AD에 employeeId가 같은 두 사용자가 있으며 서비스에서 동일한 원본 항목에 대한 중복 대상 항목을 나타내는 오류 코드를 반환합니다.

단일 사용자 및 그룹에 대한 로그를 검토하려면 특정 사용자와의 문제 프로비저닝 로그 [검토를 참조합니다.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)
