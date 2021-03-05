---
title: 사용자 프로비전
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
- "9004348"
- "8428"
ms.openlocfilehash: bd415b2d44bccf0c2b3eccb4e38452498b748b3a
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430776"
---
# <a name="user-provisioning"></a>사용자 프로비전

- 요구 [사항](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) 프로비저닝 기능을 사용하여 사용자를 프로비전하고 수행된 단계에 대한 자세한 진단을 얻을 수 있습니다.
- 사용자 및 그룹을 프로비전할 때 발생하는 문제를 해결하려면 문제 해결 가이드 [프로비전 중인 사용자가 없습니다](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned)를 참조하세요.
- 사용자가 프로비전되지 않는 것으로 확인되는 경우 Azure AD(Active Directory)에서 [로그 프로비전(미리 보기)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)을 참조하세요. 특정 사용자와 관련한 로그 항목을 검색합니다.
- 이전 프로비전 주기에서 누락된 사용자를 catch하기 위해 주기적으로 프로비전을 다시 시작합니다.
- 서비스에서 아직 사용자를 평가할 기회가 없는 경우 사용자/그룹이 프로비전되지 않았을 수 있습니다. 프로비전에 걸리는 시간 및 프로비저닝 구성 페이지의 진행률 표시줄에 대한 지침을 검토합니다. 추가 세부 정보 섹션에 지정된 상태가 사용자가 생성/업데이트/삭제된 날짜 이전인 경우 아직 사용자를 평가하지 않은 것입니다. 이 시나리오에서 가장 좋은 일은 프로비저닝 서비스가 완료될 때까지 기다리는 것입니다. 꾸준한 상태를 달성한 경우 Azure Portal의 UI에서 다시 시작을 수행하는 것이 좋습니다.
  - 서비스에서는 원본 시스템(Azure Active Directory)의 사용자/그룹 변경 내용만 인식합니다. 응용 프로그램에서 사용자/그룹이 직접 제거된 경우(예: ServiceNow) 이러한 변경 내용을 인식하지 못하며 원본 시스템의 사용자 상태를 기반으로 롤백하지 않습니다. 이 시나리오에서는 대상 응용 프로그램에서 직접 변경을 롤백하는 것이 가장 좋습니다.
- 당사의 서비스는 사용자/그룹을 평가하고 프로비전하지 않는 것으로 결정했습니다.
  - 범위를 할당된 사용자 및 그룹으로 설정한 경우 사용자/그룹이 응용 프로그램에 할당되어 있는지 검사합니다.
  - 사용자/그룹이 응용 프로그램에 할당된 경우 기본 액세스 역할에 할당되지 않은지 확인 이 역할은 프로비전에 사용할 수 없습니다.
  - 특성 기반의 지정 필터를 설정한 경우 사용자가 지정한 조건을 충족하는지 확인
  - 사용자가 대상 시스템에 이미 있으며 원본 및 대상 일치의 사용자 상태가 일치하는 경우 추가 작업을 수행하지 않습니다.
- 서비스가 사용자를 프로비전하려고 했지만 실패했습니다. 이러한 시나리오의 경우 프로비저닝 로그의 문제 해결 및 권장 사항 탭을 검토합니다.
  - 사용자의 필수 특성이 Azure Active Directory에 누락되거나 타사 응용 프로그램에서 요구하는 형식과 일치하지 않을 수 있습니다. 예를 들어 사용자의 Country 특성은 미국으로 설정될 수 있습니다.
  - 특성은 대상 응용 프로그램에 아직 없는 참조 특성입니다. referential 특성은 그룹의 구성원인 사용자와 같은 다른 개체를 포인트로 하는 특성입니다. 사용자의 ID는 그룹의 구성원 특성에 있지만 대상 사용자 개체가 이미 있는 경우만 처리될 수 있습니다.
