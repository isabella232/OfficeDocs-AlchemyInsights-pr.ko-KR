---
title: AD 사용자 프로비전 작업일이 격리 상태로 변함
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
- "8471"
- "9004687"
ms.openlocfilehash: 32a5d010b95b9587e121ca1526def743fd8f371b13d1d73d3578c692839edf19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036498"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>AD 사용자 프로비전 작업일이 격리 상태로 변함

**AD 사용자 프로비전 작업일이 격리 상태로 변하고 AD에서 사용자가 생성되지 않음**

AD 사용자 프로비전 작업일 작업이 격리 상태로 변하고 감사 로그에 다음 오류 메시지를 포함한 내보내기 실패 이벤트가 표시됩니다. **오류: OperationsError-SvcErr: 작업 오류가 발생했으므로 디렉터리 서비스에서 이 포리스트 외부의 개체에 대한 추천을 발급할 수 없습니다**. 이 오류는 일반적으로 Active Directory 컨테이너 OU가 올바르게 설정되지 않았거나 **parentDistinguishedName** 에 사용된 식 매핑에 문제가 있는 경우에 나타납니다.

**새 사용자** 매개 변수의 기본 OU에 오타가 있는지 확인합니다. 지정한 OU가 AD에 이미 존재하는지 확인합니다. 특성 매핑에서 **parentDistinguishedName** 을 사용하는 경우 항상 AD 도메인 내의 알려진 컨테이너로 평가해야 합니다. 감사 로그의 내보내기 이벤트에서 생성된 값을 확인합니다.

자동 프로비전 작업일을 구성하는 방법에 대한 자세한 내용은 [자습서: 자동 사용자 프로비전 작업일 구성](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)을 참조하세요.

