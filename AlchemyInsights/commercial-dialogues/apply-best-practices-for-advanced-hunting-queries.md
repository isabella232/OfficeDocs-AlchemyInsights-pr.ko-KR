---
title: 고급 헌팅 쿼리에 대한 모범 사례 적용
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
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736858"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>고급 헌팅 쿼리에 대한 모범 사례 적용

복잡한 쿼리를 실행하는 동안 결과를 빠르게 처리하고 시간 제한을 방지하기 위해 다음과 같은 모범 사례를 적용합니다.

- 새 쿼리를 시도할 때 항상 제한을 사용하여 결과 집합이 너무 크지 않도록 합니다. 또한 결과 집합의 크기를 초기에 `count` 평가하는 데도 사용할 수 있습니다.
- 먼저 시간 필터를 사용합니다. 이상적으로는 쿼리를 7일로 제한하는 것이 좋습니다.
- 쿼리의 시작에서 시간 필터 바로 다음에 대부분의 데이터를 제거할 것으로 예상되는 필터를 추가합니다.
- 전체 토큰을 찾는 경우 대신 `has` 연산자를 사용 `contains` 합니다.
- 모든 열이 아닌 특정 열에서 검색을 실행합니다.
- 테이블을 조인할 때 먼저 행 수가 적은 테이블을 지정합니다.
- `project` 조인한 테이블의 필수 열만

자세한 내용은 고급 헌팅 쿼리 [모범 사례를 참조합니다.](https://go.microsoft.com/fwlink/?linkid=2144812)
