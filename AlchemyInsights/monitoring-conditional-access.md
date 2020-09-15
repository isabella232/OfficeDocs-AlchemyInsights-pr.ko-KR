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
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702909"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Exchange에 대 한 조건부 액세스 모니터링

조건부 액세스를 사용 하는 사용자는 조직의 액세스 요구 사항을 충족 하지 않는 경우 알림 전자 메일을 받게 됩니다. 이 문제를 해결 하려면 다음 해결 방법 중 하나 이상을 수행 하는 것이 좋습니다.
  
- 디바이스가 등록 된 것으로 보이면 사용자에 게 회사 포털 앱으로 이동 하 여 회사 포털에 표시 되는지 확인 하도록 권고 합니다. 그렇지 않으면 사용자가 장치를 등록 해야 합니다.
    
- Azure portal에서 **Intune \> 장치 준수**로 이동 합니다. **모니터** 에서 **장치 준수**를 클릭 합니다. 장치 준수 보고서를 확인 하 여 사용자의 장치가 호환 되는 것으로 표시 되어 있는지 확인 합니다. 
    
- Azure portal에서 **Intune \> 장치 준수**로 이동 합니다. **관리**에서 **정책을**클릭 합니다. 준수 정책 목록에서 사용자의 장치에 프로필이 할당 되었는지 확인 합니다. 프로필이 할당 되지 않은 경우 Intune에서 장치의 준수 상태를 확인할 수 없습니다. 
    
- 사용자의 조건부 액세스 할당을 편집 합니다.
    
1. Azure portal에서 **Intune \> 조건부 액세스 \> 정책** 으로 이동 합니다.
    
2. 목록에서 정책 선택
    
3. **사용자 및 그룹을** 클릭 합니다.
    
4. 특정 정책을 대상으로 지정 하려면 **포함** 목록에 사용자를 추가 합니다. 정책이 정책에서 생략 되도록 하려면 해당 사용자를 **제외** 목록에 추가 합니다. 
    
자세한 내용은 다음을 참조 하십시오. [조건부 액세스 장치 모니터링 방법](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

