---
title: 모든 전자 메일 catch 만들기
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712992"
---
# <a name="create-an-email-catch-all"></a>모든 전자 메일 catch 만들기

대부분의 경우에는 catch를 사용 하지 않는 것이 좋습니다. 보낸 사람에 게 다시 바운스를 제공 하 여 보낸 사람에 게 메시지를 배달 하 여 작업을 수행할 수 있는 것으로 배달할 수 없음을 알리는 것이 좋습니다. 이전에 유효한 전자 메일 주소만 확인 하도록 모니터링 된 사서함을 제한할 수도 있습니다. 

모든 사서함을 파악 하면 적절 한 스팸을 받게 되며 면밀 하 게 모니터링 되지 않으면 결국 채워질 수도 있습니다. (수신 제한이 있습니다.) 

계속 하려면 다음 단계를 수행 합니다.

1. "모든 받는 사람 유형"을 포함 & 동적 메일 그룹을 만듭니다.

2. Catchall@domain.com과 같은 전자 메일을 catch 하기 위한 전용 사서함을 만듭니다.

3. 특정 도메인에 대해 DomainType을 "InternalRelay"로 설정 합니다. 나중에 모두 처리를 제거 하는 경우 도메인을 다시 신뢰할 수 있는 것으로 설정 해야 합니다.

4. 메일 흐름 전송 규칙을 만드는 방법은 다음과 같습니다.

    - 보낸 사람이 "조직 외부" 인 경우
    - 메시지를 Catchall@domain.com로 리디렉션
    - 받는 사람이 allusers@domain.com의 구성원 인 경우 제외 (모든 구성원이 포함 된 메일 그룹)
    - 동적 메일 그룹에 새 사서함이 추가 되었는지 확인 합니다.
