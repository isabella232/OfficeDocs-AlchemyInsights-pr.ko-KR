---
title: 보고서를 여는 데 기존 대화 포함 사용
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: 285933e607ac7e58256709f0c9cf2851250ce211
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806441"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>보고서를 여는 데 기존 대화 포함 사용

**증상**

사용자가 보고서를 열 수 없습니다. "문제가 발생했습니다. 자세한 내용은 기술 세부 사항을 확인하세요."

**원인**

"양식 디스크립터가 NULL이거나 정의되지 않음" 오류와 함께 UCI에서 보고서를 로드하지 못했습니다. UCI에서 보고서를 사용하려면 기존 대화가 계속 필요하므로, 고객의 시스템에 *allowlegacydialogsembedding*이 활성화되어 있어야 합니다.

**솔루션**

1. **설정 > 관리 > 시스템 설정 > 일반 탭**으로 이동합니다.

2. "통합 인터페이스 브라우저에서 특정 레거시 대화 포함 사용"을 **예**로 설정합니다.
