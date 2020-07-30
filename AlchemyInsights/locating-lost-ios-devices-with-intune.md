---
title: Intune을 사용하여 분실된 iOS 장치 찾기
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434596"
---
# <a name="locating-lost-ios-devices-with-intune"></a>Intune을 사용하여 분실된 iOS 장치 찾기

iOS 장치에서 분실 모드를 사용하도록 설정하면 관리자가 잠금 화면에 메시지와 연락처 전화 번호를 표시할 수 있습니다.

분실 모드를 사용하도록 설정한 후 관리자가 장치 찾기 작업을 사용하여 장치의 실제 위치를 확인할 수 있습니다.

Intune의 장치 찾기 작업은 iOS 장치에서 작동하여 지도에서 특정 장치의 위치를 표시합니다.

이 작업을 사용하려면 iOS 장치에서 다음을 사용해야 합니다.

- 감독 모드
- 분실 모드

자세한 내용은 [Intune을 사용하여 iOS/iPadOS 장치에서 분실 모드 사용](https://docs.microsoft.com/intune/device-lost-mode) 및 [Intune을 사용하여 분실하거나 도난당한 iOS/iPadOS 장치 찾기](https://docs.microsoft.com/intune/device-locate)를 참조하세요.

**FAQ**

Q: 장치에서 회사 데이터를 제거하기 위한 원격 작업을 실행했는데, 현재 계속 보류 상태입니다.

A: 원격 작업이 성공적으로 완료되려면 대상 장치가 온라인 상태여야 합니다. 다음과 같은 경우 원격 작업은 30일 동안 또는 장치가 명령을 인식할 때까지 보류 상태로 유지됩니다.

- 장치에 연결할 수 없는 경우
- 장치가 Intune에서 관리 상태가 누락되는 경우

장치가 더 이상 체크인하지 않고 회사 데이터를 제거할 수 없는 경우, 삭제를 선택합니다. 삭제하면 장치 레코드가 제거되어 장치의 Intune 목록에 더 이상 나타나지 않습니다. 장치가 다시 활성화되면 사용자가 이를 다시 등록해야 합니다.

Q: 특정 원격 작업을 사용할 수 없는 이유는 무엇입니까?

A: 모든 플랫폼이 모든 원격 장치 작업을 지원하는 것은 아닙니다. 다음 원격 작업은 플랫폼에 따라 달라지며 언급된 플랫폼에서만 사용할 수 있습니다.

- 활성화 잠금을 바이패스합니다(iOS만 해당).
- 새로 시작합니다(Windows 전용).
- 모드가 손실되었습니다(iOS만 해당).
- 장치를 찾습니다(iOS만 해당).
- 다시 시작합니다(Windows 전용).

각 작업에 대한 자세한 내용은 [사용 가능한 디바이스 작업](https://docs.microsoft.com/intune/device-management#available-device-actions)을(를) 참조합니다.