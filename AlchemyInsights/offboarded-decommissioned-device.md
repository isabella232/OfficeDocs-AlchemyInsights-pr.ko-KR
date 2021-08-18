---
title: 장치 인벤토리에서 오프보딩되거나 해제된 장치를 제거하는 데 문제가 있습니다.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 13865acb75b60a824c1dde9427c11471e980ea9e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324450"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a>장치 인벤토리에서 오프보딩되거나 해제된 장치를 제거하는 데 문제가 있습니다.

끝점용 Microsoft Defender는 현재 장치 인벤토리에서 오프보딩 또는 해제된 장치의 장치 레코드를 수동으로 제거할 수 없습니다.

보안을 위해 장치는 포털에 최대 180일 동안 기록 레코드로 남아 있습니다. 그러나 구성된 보존 기간에 따라 장치 데이터가 제거됩니다.

**참고:** 오프보딩되거나 해제된 장치는 7일  후에 자동으로 비활성 상태로 전환됩니다. 또한 지난 30일 동안 활성화되지 않은 장치는 조직이 노출 점수 또는 장치에 대한 Microsoft 보안 점수를 위협 및 취약성 관리 데이터를 고려하지 않습니다.
 
여전히 장치 인벤토리 보기에서 특정 장치를 보고 싶지 않은 경우 장치 태그를 배치하여 장치 인벤토리 보기에서 해제된 장치를 필터링해 봐야 합니다.

자세한 내용은 다음을 참조하세요.

[Microsoft Defender for Endpoint Service에서 장치 오프보딩](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/offboard-machines.md)

[노출 점수(위협 및 취약성 관리](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[Endpoint용 Microsoft Defender에서 불안정한 센서 수정](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[태그 지정을 효과적으로 사용하는 방법(1부)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[태그 지정을 효과적으로 사용하는 방법(2부)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[태그 지정을 효과적으로 사용하는 방법(3부)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




