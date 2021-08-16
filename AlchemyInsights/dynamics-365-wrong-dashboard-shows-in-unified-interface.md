---
title: Dynamics 365 - Dynamics 365 통합 인터페이스에 잘못된 대시보드 표시
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 1edb2a7e9e0c270c7e98eb43d2f6514d70c39a19ea97d189322ca387b6842a18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101488"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Dynamics 365 통합 인터페이스에 잘못된 대시보드가 표시됩니다.

예상과 다른 대시보드가 표시될 수 있는 이유는 여러 가지가 있습니다.

## <a name="the-user-has-set-a-user-default-dashboard"></a>사용자가 사용자 기본 대시보드를 설정한 경우 

일반적으로 기본으로 설정 단추가 대시보드  명령 표시줄에 표시되어 있지 않은 경우 사용자 기본 대시보드가 설정되어 있는 경우를 식별할 수 있습니다. 사용자의 기본 대시보드가 현재 앱에 있지 않은 경우에도 사용자 기본 대시보드는 다른 모든 기본 대시보드를 다시 지정합니다.

다음 해결 방법을 사용하여 기본 대시보드를 설정하지 않습니다.

1. 새 개인 대시보드를 만들 수 있습니다.

2. 새 대시보드를 사용자 기본값으로 설정하세요.

3. 해당 대시보드를 삭제합니다.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>대시보드가 사이트맵에 설정되어 있습니다.

대시보드를 선택하고 '시스템 사용자 지정'에서 '기본값으로 설정'을 선택하여 조직 기본 대시보드를 설정한 것일 수 있습니다. 그러나 사용자가 사이트에 액세스할 수 있는 경우 사이트맵 디자이너에 정의된 대시보드가 이 대시보드보다 우선합니다.

조직 기본값으로 설정한 대시보드를 사용자에게 표시하기 위해 다음 중 하나를 사용할 수 있습니다.

* 사이트맵에서 대시보드 설정

* 해당 사용자에 대해 사이트맵 정의된 대시보드에 대한 액세스 제거
