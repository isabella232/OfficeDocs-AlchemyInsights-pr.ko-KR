---
title: Intune에서 데이터 삭제하고 장치 초기화
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: 92673c4a2a0e0faa98d3ade5ca1f6aa687d4c94a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331047"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Intune에서 데이터 삭제하고 장치 초기화

Intune에서 회사 데이터를 삭제하거나 공장 초기화를 실행하고 장치를 기본 설정으로 되돌리기 위해 장치 사용 중지 및 장치 초기화 원격 작업을 사용 할 수 있습니다.

1. Microsoft 365 장치 관리에 로그인하고 **장치** > **모든 장치** 로 이동하세요.
2. 초기화 할 장치를 선택합니다.
3. 원하는 원격 초기화 유형을 선택합니다. 사용 중지는 조직 정보만 삭제하고 전체 초기화는 장치를 공장 설정으로 복원합니다.
4. **예** 를 선택하여 확인합니다. 장치가 삭제될 때까지 장치 활동 상태는 *사용 중지 보류 중* 으로 보여집니다.
    작업이 완료되면 관리되는 장치 목록에서 모바일 장치를 더는 볼 수 없습니다.

**참고** Azure AD에 조인된 장치에서는 회사 데이터를 제거할 수 없습니다. 

유지되는 항목 및 삭제 되는 항목을 포함하여 사용 중지 및 초기화 작업 영향에 대한 자세한 내용은

- [초기화, 사용 중지 또는 수동으로 장치 등록 삭제하기를 사용하여 장치 삭제](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe)를 참조하세요.
- [Intune 관리 앱에서 기업 데이터만 초기화하는 방법](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [macOS 장치에서 모든 데이터 지우기](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).