---
title: Dynamics 365-Dynamics 365 통합 인터페이스에 잘못 된 대시보드가 표시 됨
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
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711281"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Dynamics 365 통합 인터페이스에 잘못 된 대시보드가 표시 됨

예상과 다른 대시보드가 표시 되는 몇 가지 이유는 다음과 같습니다.

## <a name="the-user-has-set-a-user-default-dashboard"></a>사용자가 사용자 기본 대시보드를 설정 했습니다. 

**기본적으로 설정** 단추가 대시보드 명령 모음에 표시 되지 않는 경우 일반적으로 사용자 기본 대시보드가 설정 됩니다. 사용자의 기본 대시보드가 현재 앱에 없는 경우에도 사용자 기본 대시보드는 다른 모든 기본 대시보드를 재정의 합니다.

다음 해결 방법을 사용 하 여 기본 대시보드를 설정 해제할 수 있습니다.

1. 새 개인 대시보드를 만듭니다.

2. 새 대시보드를 사용자 기본값으로 설정 합니다.

3. 대시보드를 삭제 합니다.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>대시보드는 사이트 맵에서 설정 됩니다.

대시보드를 선택 하 고 ' 시스템 사용자 지정 ' 아래의 ' 기본값으로 설정 '을 선택 하 여 조직 기본 대시보드를 설정 했을 수 있습니다. 하지만 사이트 맵 디자이너에 정의 된 대시보드는 사용자가 액세스할 수 있는 경우이 대시보드 보다 우선 합니다.

사용자가 조직 기본값으로 설정한 대시보드를 볼 수 있도록 하려면 다음 중 하나를 수행 합니다.

* 사이트 맵에서 대시보드 설정

* 해당 사용자에 대 한 사이트 맵 정의 대시보드에 대 한 액세스 권한 제거
