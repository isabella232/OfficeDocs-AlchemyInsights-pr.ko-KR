---
title: 소프트웨어 인벤터리가 없거나 부정확 합니다.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52658053"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a>소프트웨어 인벤터리가 없거나 부정확 합니다.

위협 및 TVM(취약성 관리)의 소프트웨어 인벤토리는 공식 CPE(공통 플랫폼 열거)가 있는 조직의 알려진 소프트웨어 목록입니다.

공식 CPE가 없는 소프트웨어 제품에는 취약성이 게시되지 않았습니다. 인벤토리에는 공급업체 이름, 취약점 수, 위협 및 노출된 장치 수와 같은 세부 정보도 포함됩니다.

장치의 소프트웨어 변경 사항은 일반적으로 보안 포털에 2시간 이내에 반영됩니다. 하지만, 때때로 더 오래 걸릴 수도 있습니다. 현재 동기화를 강제할 수 있는 방법은 없습니다. 지속적인 평가입니다.

소프트웨어를 변경했는데 5시간 후에 변경 사항이 TVM에 정확하게 반영되지 않는 경우 다음 단계를 수행하세요.

1. 소프트웨어 증거 섹션을 확인하여 소프트웨어가 어떻게 감지되었는지 알아보세요.
1. 소프트웨어가 지원되는지 확인합니다. 소프트웨어는 현재 위협 및 취약성 관리에서 지원되지 않는 경우에도 장치 수준에서만 볼 수 있습니다. 그러나 제한된 데이터만 사용할 수 있습니다.
1. 포털에서 부정확성을 보고하는 단계는 [부정확성 보고](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy)를 참조하세요.
   
    **참고**: MDE 포털에서 부정확성을 보고하는 것은 엔지니어링을 위한 단방향 채널입니다. 문제가 긴급하면 지원 티켓을 여세요.

더 자세한 내용은 [소프트웨어 인벤토리 - 위협 및 취약성 관리](/microsoft-365/security/defender-endpoint/tvm-software-inventory)를 참조하세요.