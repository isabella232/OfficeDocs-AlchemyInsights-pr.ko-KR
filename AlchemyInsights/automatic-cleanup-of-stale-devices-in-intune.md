---
title: Intune에서 오래 된 장치 자동 정리
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/28/2020
ms.locfileid: "46505204"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Intune에서 오래 된 장치 자동 정리

Intune에서는 관리자가 서비스에서 오래 된 장치를 제거한 후 90일에서 270일 사이의 시간 간격 구성을 허용 합니다. 조직 전체 설정이며 활성화 되면 즉시 적용됩니다. 설정을 초과 하는 기간 동안 Intune 서버에 체크인하지 않은 장치는 영구적으로 삭제됩니다.

**참고** MDM 장치 개체만 정리 할 수 있습니다. EAS 단독 장치 개체는 제외 됩니다.

장치 정리 설정 및 해당 "상태"를 기준으로한 장치 삭제에 대한 자세한 내용은 다음을 참조하세요.

설정: **마지막 체크인 날짜 후 장치 삭제: 예(일부 특정 날짜 값 (N))**

- 설정에서 구성한 값(N)을 기준으로하여 마지막으로 체크인 된 장치가 지정된 날짜를 지나면 Intune에서 해당 장치를 삭제합니다.

설정: **마지막 체크인 날짜 이후 장치 삭제: 아니요**

- 장치가 인증 된지 180일이 지나고 갱신되지 않으면 장치가 삭제됩니다.

**참고** 두 경우 모두 장치가 Intune에 등록되어 있어야 합니다. 등록은 Intune 서비스에 처음으로 장치를 체크인 할 때 이루어집니다.

장치가 Intune에 등록 되었지만 Intune 등록 장치가 되지 않는 경우 장치는 등록 후 270일 이내에 삭제됩니다. (90일에 해당 장치가 해지 된 것으로 표시하고 향후 180일 이후에는 기록을 삭제합니다.)

현재 어떤 장치에도 Intune 콘솔에 장치 인증 만료 날짜를 설정하는 장치가 존재하지 않습니다.