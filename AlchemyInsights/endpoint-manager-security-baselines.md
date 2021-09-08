---
title: Endpoint Manager - 보안 기준
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: 4c8e03a817751ba7dc1710aed5a3e19c6e79db33
ms.sourcegitcommit: ae556b6b26974392ca68a68426a2b40967ae0071
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/07/2021
ms.locfileid: "58923560"
---
# <a name="endpoint-manager---security-baselines"></a>Endpoint Manager - 보안 기준

보안 기준은 관련 보안팀에서 권장하는 보안 설정을 적용할 수 있도록 미리 구성된 Windows 설정 그룹입니다. 이러한 기준은 원하는 설정과 값만 제공하도록 사용자 지정될 수 있습니다. 보안 기준에 대한 자세한 내용은 [보안 기준을 사용하여 Intune에서 Windows 10 장치 구성](https://docs.microsoft.com/mem/intune/protect/security-baselines)을 참조하세요.

현재 다음 제품에 대한 기준이 있습니다.

- Windows MDM 보안 설정
- 엔드포인트용 Microsoft Defender  보안
- Microsoft Edge

각 기준은 주기적으로 업데이트되어 증분 버전으로 릴리스됩니다. 각 버전은 기준이 현재 지침을 충족하도록 이전 버전에서 설정을 추가하거나 제거합니다. Endpoint 보안의 보안 기준 콘솔을 사용하면 버전 간 변경 내용을 표시하여 서로 다른 버전을 비교할 수 있습니다.

배포된 기준의 버전을 가장 효과적으로 변경하는 방법에 대한 지침은 [Microsoft Intune에서 보안 기준 프로필 관리](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)를 참조하세요.

보안 기준을 배포한 후 배포 상태를 모니터링하고 장치 기준에 따라 설정을 검토할 수 있습니다.

보안 기준에는 많은 설정이 포함되어 있으므로 구성 변경을 검토하고 모든 설정이 장치 및 비즈니스 요구 사항에 적합한지 테스트를 수행하는 것이 중요합니다.

**참고:** 기준에 대한 데이터를 보고하는 경우 초기 배포에서 장치에 표시되는 데 최대 24시간, 추가 업데이트에 최대 6시간이 걸릴 수 있습니다. 

기준 설정이 적용되지 않는 가장 일반적인 원인은 다른 프로필에서 동일한 설정을 사용하기 때문입니다. 이 시나리오는 보안 기준 프로필의 장치 상태 노드에서 장치를 선택하여 특정 장치에 대해 조사할 수 있습니다. 자세한 내용은 [보안 기준에 대한 충돌 해결](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)을 참조하세요.