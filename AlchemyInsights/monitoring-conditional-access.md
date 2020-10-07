---
title: 조건부 액세스 모니터링
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366434"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Exchange에 대 한 조건부 액세스 모니터링

조건부 액세스를 사용 하는 사용자는 조직의 액세스 요구 사항을 충족 하지 않는 경우 알림 전자 메일을 받게 됩니다. 이 문제를 해결 하려면 다음 해결 방법 중 하나 이상을 수행 하는 것이 좋습니다.

- 디바이스가 등록 된 것으로 보이면 사용자에 게 회사 포털 앱으로 이동 하 여 회사 포털에 표시 되는지 확인 하도록 권고 합니다. 그렇지 않으면 사용자가 장치를 등록 해야 합니다.
- Azure portal에서 Intune > 장치 준수로 이동 합니다. 모니터에서 장치 준수를 클릭 합니다. 장치 준수 보고서를 확인 하 여 사용자의 장치가 호환 되는 것으로 표시 되어 있는지 확인 합니다.
- Azure portal에서 Intune > 장치 준수로 이동 합니다. 관리에서 정책을 클릭 합니다. 준수 정책 목록에서 사용자의 장치에 프로필이 할당 되었는지 확인 합니다. 프로필이 할당 되지 않은 경우 Intune에서 장치의 준수 상태를 확인할 수 없습니다.
- 사용자의 조건부 액세스 할당을 편집 합니다.

1. Azure portal에서 **Intune**  >  **조건부 액세스**  >  **정책**으로 이동 합니다.
2. 목록에서 정책을 선택 합니다.
3. 사용자 및 그룹을 클릭 합니다.
4. 특정 정책을 대상으로 지정 하려면 포함 목록에 사용자를 추가 합니다. 정책이 정책에서 생략 되도록 하려면 해당 사용자를 제외 목록에 추가 합니다.

유용한 링크:

[장치 준수 개요](https://docs.microsoft.com/intune/device-compliance-get-started)

[CA 문제 해결](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[문제 해결 정책](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[Intune 장치 준수 모니터링](https://docs.microsoft.com/intune/compliance-policy-monitor)

참고: 이러한 단계는 Azure Active Directory 기능 조건부 액세스 문제를 해결 하는 경우에만 유용 합니다. Exchange 정책과의 전자 메일 액세스를 차단 하는 장치를 격리 하는 것도 가능 합니다. Exchange 장치 관리에 대 한 자세한 내용은 [여기](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>)에서 확인할 수 있습니다.
