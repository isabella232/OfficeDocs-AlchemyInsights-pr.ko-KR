---
title: 복제 데이터베이스 집합
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 45cf530c3258fa3c7008c3e8251fdb7b74be6911d0487f58c5ce2530e25ca282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54110686"
---
# <a name="replica-set"></a>복제 데이터베이스 집합

AADDS를 관리되는 도메인이라고도 합니다. 실제로 백end에서 실행 및 유지 관리하는 도메인 컨트롤러 두 개입니다. 두 개의 DC에는 하나의 주 DC와 하나의 복제 DC가 포함됩니다. AADDS(관리되는 도메인)의 백업은 Azure 플랫폼에서 관리하는 자동화된 프로세스입니다. 관리되는 도메인에 문제가 발생하면 Azure 지원이 백업에서 복원하는 데 도움이 될 수 있습니다.

가상 네트워크에서 각 복제 데이터베이스 집합을 만들 수 있습니다. 각 가상 네트워크는 관리되는 도메인의 복제본 집합을 호스트하는 다른 모든 가상 네트워크와 피어링되어야 합니다. 이 구성에서는 디렉터리 복제를 지원하는 메시 네트워크 토폴로지가 생성됩니다. 각 복제 데이터베이스 집합이 다른 가상 서브넷에 있는 경우 가상 네트워크에서 여러 복제 데이터베이스 집합을 지원할 수 있습니다.

복제 데이터베이스 집합에 대한 자세한 내용은 개념 복제본 [집합 을 참조합니다.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)
