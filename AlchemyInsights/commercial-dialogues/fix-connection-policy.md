---
title: 연결 정책 수정
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: d27d570a7bc0f2c1081ba7fd52264a20bf25a453
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314850"
---
# <a name="fix-connection-policy"></a>연결 정책 수정

원본 IP 주소가 기본 연결 필터 정책에서 안전한 것으로 표시되어 전자 메일이 안전한 것으로 표시되어 사용자의 받은 편지함으로 배달됩니다. 정책을 검토하기 위해 다음 단계를 수행합니다.

1. 의 Microsoft 365 Defender 포털에서 전자 메일 & 공동 작업 정책 & 규칙 위협 정책 스팸 방지 <https://security.microsoft.com/>  \>  \>  \>  **섹션으로** 이동하세요.

   **스팸 방지 정책** 페이지로 직접 이동하려면 <https://security.microsoft.com/antispam>을(를) 사용합니다.

2. 스팸 **방지 정책 페이지에서** 정책 이름을 클릭하여 연결 필터 정책(기본값)이라는 정책을 선택합니다. 

3. 세부 정보 플라이아웃이 나타나면 연결 필터링 섹션에서 연결 필터 **정책** **편집을** 클릭합니다.

4. 다음 **IP** 주소 또는 주소 범위에서 항상 메시지 허용 섹션의 항목을 검토하고 수신 허용 목록 설정이 **선택되어** 있는지 검토합니다.

   **참고:** Microsoft는 신뢰할 수 있는 보낸 사람에 대한 타사 소스를 구독합니다. 수신 확인 목록이 사용하도록 설정된 경우 이러한 신뢰할 수 있는 보낸 사람이 스팸으로 잘못 표시되지 않습니다. 받는 가음성(스팸으로 분류된 양호한 메일)의 수가 줄어들기 때문에 이 옵션을 선택하는 것이 좋습니다.

자세한 내용은 [연결 필터링 구성](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy)을 참조하십시오.
