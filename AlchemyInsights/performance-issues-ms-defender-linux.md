---
title: Linux의 엔드포인트용 Microsoft Defender 성능 문제
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: b1200f0dd206e27cccf96778beb0326c846e7504e51be283193b2630edfb4509
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086746"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>Linux의 엔드포인트용 Microsoft Defender 성능 문제

이 문서에서는 Linux의 엔드포인트용 Microsoft Defender에 대한 성능 문제를 식별하는 단계를 안내합니다.

먼저 발생한 문제가 [최신 버전](/microsoft-365/security/defender-endpoint/linux-whatsnew)으로 해결되었는지 확인하는 것이 중요합니다. 

조사를 시작하려면 [Linux의 엔드포인트용 Microsoft Defender의 성능 문제 해결](/microsoft-365/security/defender-endpoint/linux-support-perf)을 참조하세요.

## <a name="exclusions"></a>제외

제외는 성능 문제를 완화하는 데 도움이 될 수 있습니다. 추가 위험이 파악되고 문서화되도록 시작하기 전에 제외 사항을 검토하세요.

자세한 내용은 [Linux의 엔드포인트용 Microsoft Defender에 대한 제외 구성 및 유효성 검사](/microsoft-365/security/defender-endpoint/linux-exclusions)를 참조하세요.

제외할 파일 및 폴더가 여러 개 있고 모두 동일한 마운트 지점에 있는 경우 마운트 지점을 제외하는 것이 더 쉬울 수 있습니다. 2월 릴리스 101.22.80부터 전체 마운트 지점을 제외할 수 있습니다.

예를 들어 /mnt/backup이 마운트 지점인 경우 다음 명령을 실행하여 제외 목록에 /mnt/backup을 추가할 수 있습니다.

`$ mdatp exclusion folder add –path /mnt/backup`

**참고**: 제외 항목을 추가하면 맬웨어가 탐지되지 않을 위험이 증가하므로주의해서 처리하고 구현해야 합니다.

## <a name="need-help"></a>도움이 필요하세요?

가장 효율적인 방법으로 지원하려면 지원 케이스를 열기 전에 진단 데이터를 수집하세요.
