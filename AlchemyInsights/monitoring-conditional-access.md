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
ms.openlocfilehash: 80e8cc72db8ae32445d48e5c8a411d5ccd538626653260b3dbd28a247561e888
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975107"
---
# <a name="monitoring-conditional-access-for-exchange"></a>사용자에 대한 조건부 액세스 Exchange

조건부 액세스를 대상으로 하는 사용자는 조직의 액세스 요구 사항을 충족하지 않는 경우 알림 전자 메일을 받게 됩니다. 해결을 위해 다음 솔루션 중 하나 이상을 해결하는 것이 좋습니다.

- 디바이스가 등록된 것으로 생각되는 경우 사용자에게 회사 포털 앱으로 이동하여 디바이스가 앱에 나타나는지 회사 포털. 그렇지 않은 경우 사용자는 장치를 등록해야 합니다.
- Azure Portal에서 Intune > 장치 준수로 이동하세요. 모니터에서 장치 준수를 클릭합니다. 장치 준수 보고서를 보고 사용자의 장치가 규격으로 표시되어 있는지 확인합니다.
- Azure Portal에서 Intune > 장치 준수로 이동하세요. 관리에서 정책을 클릭합니다. 준수 정책 목록에서 프로필이 사용자의 장치에 할당되어 있는지 확인합니다. 프로필이 할당되지 않은 경우 Intune에서 장치의 준수 상태를 확인할 수 없습니다.
- 사용자의 조건부 액세스 할당을 편집합니다.

1. Azure Portal에서 **Intune**  >  **조건부 액세스 정책으로**  >  **이동하세요.**
2. 목록에서 정책을 선택합니다.
3. 사용자 및 그룹을 클릭합니다.
4. 누군가의 특정 정책을 대상으로 지정하기 위해 포함 목록에 추가합니다. 사용자가 정책에서 생략되도록 제외 목록에 추가합니다.

유용한 링크:

[장치 준수 개요](https://docs.microsoft.com/intune/device-compliance-get-started)

[CA 문제 해결](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[문제 해결 정책](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Intune 장치 준수 모니터링](https://docs.microsoft.com/intune/compliance-policy-monitor)

참고: 이러한 단계는 조건부 액세스 기능의 Azure Active Directory 유용합니다. 또한 장치 정책을 사용하여 전자 메일 액세스를 차단하는 장치를 Exchange 있습니다. 장치 관리에 Exchange 자세한 내용은 [here]( 을(를) 찾을 수 https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) 있습니다.
