---
title: Defender 엔드포인트 확인 센서 상태
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: cefebe63e45caab176ba84a35280378ace7e6b3115c48694ed043a39b4d93c1e
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890060"
---
# <a name="defender-endpoint-check-sensor-status"></a>Defender 엔드포인트 확인 센서 상태

**센서 문제가 있는 장치** 타일이 보안 작업 대시보드에 있습니다. 이 타일은 개별 장치에서 센서 데이터를 제공하고 엔드포인트용 Defender 서비스와 통신하는 기능의 정보를 제공합니다. 주의가 필요한 장치 수를 보고하고 문제가 있는 장치를 식별하고 알려진 문제를 수정하기 위한 조치를 취하는 데 도움이 됩니다.

타일의 두 상태 표시기는 서비스에 제대로 보고하지 않는 장치 수에 대한 정보를 제공합니다.

- 부분적으로 엔드포인트용 Defender 서비스에 센서 데이터를 보고하고 있을 수 있으며 수정해야 하는 구성 오류가 있을 수 있는 **잘못 구성된** 장치입니다.
- 지난 달에 7일 이상 엔드포인트용 Defender 서비스에 보고를 중지한 **대화 불가능** 장치입니다.

그룹을 클릭하면 선택에 따라 필터링된 장치 목록으로 연결됩니다. 장치 목록에서 다음 상태로 상태 목록을 필터링할 수 있습니다.

- 엔드포인트용 Defender 서비스에 활발히 보고하고 있는 **대화 가능** 장치입니다.
- 부분적으로 엔드포인트용 Defender 서비스에 센서 데이터를 보고하고 있을 수 있으나 수정해야 하는 구성 오류가 있는 **잘못 구성된** 장치입니다. 잘못 구성된 장치에는 다음 문제 중 하나 또는 문제의 조합이 있을 수 있습니다.

    - 센서 데이터가 없습니다. 장치가 센서 데이터 전송을 중지했습니다. 장치에서 제한된 경고를 트리거할 수 있습니다.
    - 통신 장애 - 장치와 통신하는 기능이 손상되었습니다. 심층 분석을 위한 파일 전송, 파일 차단, 네트워크에서 장치 분리, 장치와 통신이 필요한 기타 작업이 작동하지 않을 수 있습니다.
- 엔드포인트용 Defender 서비스에 보고를 중지한 **대화 불가능** 장치입니다.

내보내기 기능을 사용하여 CSV 형식으로 전체 목록을 다운로드할 수 있습니다.

자세한 내용은 [엔드포인트용 Microsoft Defender에서 센서 상태 확인](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/check-sensor-status)을 참조하세요.

장치가 대화가 불가능하게 되거나 잘못 구성된 원인에 대한 자세한 내용은 [엔드포인트용 Microsoft Defender에서 비정상 센서 수정](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)을 참조하세요.
