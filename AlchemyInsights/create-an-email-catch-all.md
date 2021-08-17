---
title: 전자 메일 catch 모두 만들기
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 0d20f7bcffa3be43fc6186a938bf4a7338722f5cd225b860da6357398db26a69
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080752"
---
# <a name="create-an-email-catch-all"></a>전자 메일 catch 모두 만들기

catch를 모두 사용하는 것은 강력히 금지됩니다. 보낸 사람이 조치를 취할 수 있도록 보낸 사람이 메시지를 주소로 배달할 수 없다고 알려주는 반송을 보낸 사람에 제공하는 것이 좋습니다. 모니터링되는 사서함이 이전의 유효한 전자 메일 주소만 catch하는 것으로 제한할 수도 있습니다. 

모든 catch 모든 사서함은 스팸을 상당 부분을 받으며 면밀하게 모니터링하지 않는 경우 결국 채울 수 있습니다. 수신 제한이 있습니다. 

계속하기로 결정한 경우 다음 단계를 수행합니다.

1. "모든 받는 사람 유형"& 메일 그룹 만들기

2. 예를 들어 전자 메일을 catch하기 위한 전용 사서함을 catchall@domain.com.

3. 특정 도메인의 경우 DomainType을 "InternalRelay"로 설정합니다. 나중에 catch를 모두 제거하는 경우 도메인을 다시 Authoritative로 설정해야 합니다.

4. 다음과 같이 메일 흐름 전송 규칙을 만들 수 있습니다.

    - 보낸 사람이 "조직 외부"인 경우
    - 메시지를 메시지로 Catchall@domain.com
    - 받는 사람이 allusers@domain.com 구성원인 경우를 제외하고(메일 그룹에 모든 구성원 포함)
    - 새 사서함이 동적 메일 그룹에 추가되는지 확인
