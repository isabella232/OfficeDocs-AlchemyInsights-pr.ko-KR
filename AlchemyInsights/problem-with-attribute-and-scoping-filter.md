---
title: 특성 및 범위 지정 필터에 문제가 있는 경우
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 51ed0fabe220d0069d721ec64d049787bacd5b094e19f0c1996a28e07bb56f03
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960193"
---
# <a name="problem-with-attribute-and-scoping-filter"></a>특성 및 범위 지정 필터에 문제가 있는 경우

**UPN 값 충돌 문제**

Workday ~ AD 사용자 프로비전 Workday ~ AD 사용자 프로비전 작업 시 **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique** 오류 메시지가 표시됩니다. 추가/수정을 위해 입력한 UPN 값이 포리스트 범위에서 고유하지 않아서 작업이 실패했습니다. 오류 세부 정보: **CONSTRAINT_ATT_TYPE - userPrincipalName**.

AD 사용자 계정을 만들 때 Workday 커넥터에서 설정하려고 하는 **userPrincipalName** 값이 대상 AD 도메인에 이미 존재합니다. 즉, (1) 사용자가 이미 존재하며 해당 사용자에 대한 일치하는 ID 검사가 실패했거나 (2) UPN 생성 규칙에 따라 충돌하는 값이 발생한 것입니다.

제안된 해결 단계는 다음과 같습니다.

사용자가 이미 있으며 일치하는 ID 검사에서 Workday 계정을 Active Directory 계정에 연결하지 못한 경우라면 Workday와 AD 양쪽에서 일치하는 ID 특성(일반적으로 **employeeID**)이 정확히 일치하는지 확인합니다. 일치하지 않는 경우 수정해야 하는 데이터 문제입니다. 예를 들어 Workday의 EmployeeID는 001052이고 AD의 EmployeeID는 1052라면 프로비전 엔진이 두 계정을 연결하지 못하고 이미 존재하는 사용자를 만들려고 합니다. 이 경우의 해결 방법은 AD의 **EmployeeID** 값 앞에 0을 집어넣어 001052로 되도록 변경하는 것입니다.
UPN 생성 식에서 고유 값을 생성하지 않는 경우 중복 제거 함수 **SelectUniqueValue** 를 사용하여 매번 고유한 값을 생성하게 하는 것이 고려해 보세요.

**Workday ~ AD 사용자 프로비전 작업에서 AD 사용자 계정에 대한 관리자 특성 값이 설정되지 않는 경우**

Workday ~ AD 사용자 프로비전 작업에서 AD 사용자 계정에 대한 **관리자** 특성 값을 설정하지 않습니다. 이러한 동작이 관찰되는 경우 가능한 다음 두 가지 시나리오가 있습니다.

1. 관리자는 검색 범위에 포함되지 않아 Workday의 관리자가 해당하는 AD 사용자 계정으로 해결되지 않습니다.
2. **여러 AD 도메인** 시나리오에서는 Workday의 관리자가 사용자와 동일한 도메인에 있지 않습니다.

다음 단계를 시도하여 문제를 해결하세요.

1. 범위 지정 필터를 정의한 경우 먼저 관리자가 범위 내에 있으며 범위 지정 절을 충족하는지 확인합니다. 관리자가 범위 지정 필터를 충족하지 않는 경우 관리자가 프로비전 작업의 범위에 포함되도록 필터를 변경합니다.
2. AD 도메인이 여러 개인 경우 커넥터에 도메인 간 관리자 참조를 해결하지 못하는 제한이 있는 것으로 알려졌습니다.

자동 프로비전 작업일을 구성하는 방법에 대한 자세한 내용은 [자습서: 자동 사용자 프로비전 작업일 구성](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)을 참조하세요.













