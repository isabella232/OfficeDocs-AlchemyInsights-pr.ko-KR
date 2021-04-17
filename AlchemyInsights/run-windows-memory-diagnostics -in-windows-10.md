---
title: Windows 10에서 Windows 메모리 진단 실행
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826673"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Windows 10에서 Windows 메모리 진단 실행

PC에서 Windows 및 앱이 작동을 중지하거나 멈추거나 또는 불안정한 방식으로 작동하는 경우 PC의 메모리(RAM)에 문제가 있을 수 있습니다. Windows 메모리 진단 도구를 실행하 여 PC의 RAM 문제를 확인할 수 있습니다.

작업 표시줄의 검색 상자에 **메모리 진단** 을 입력한 다음, **Windows 메모리 진단** 을 선택합니다. 

진단 도구를 실행하려면 PC를 다시 시작해야 합니다. 즉시 다시 시작하는 옵션(작업을 저장 하고 열린 문서와 전자 메일을 먼저 닫음)을 사용하거나 다음에 PC가 다시 시작될 때 진단이 자동으로 실행되도록 예약하는 옵션이 있습니다.

![Windows 메모리 진단](media/windows-memory-diagnostic.png)

PC가 다시 시작될 때, **Windows 메모리 진단 도구** 가 자동으로 실행됩니다. 진단 도구가 실행되는 동안 상태와 진행률이 표시되고 키보드에서 **ESC** 키를 눌러 진단 도구를 취소할 수 있는 옵션이 있습니다.

진단이 완료되면 Windows가 정상적으로 시작됩니다.
다시 시작된 직후에 바탕 화면이 나타나면 작업 표시줄에서 **알림 센터** 아이콘 옆에 알림이 표시되어 메모리 오류를 찾았는지 여부를 나타냅니다. 예시:

알림 센터 아이콘은 다음과 같습니다. ![알림 센터 아이콘](media/action-center-icon.png) 

샘플 알림: ![메모리 오류 없음](media/no-memory-errors.png)

알림을 놓친 경우, 작업 표시줄에 있는 **알림 센터** 아이콘을 선택하여 **알림 센터** 를 표시하고 스크롤할 수 있는 알림 목록을 볼 수 있습니다.

세부 정보를 검토하려면 작업 표시줄의 검색 상자에 **이벤트** 를 입력한 다음, **이벤트 뷰어** 를 선택합니다. **이벤트 뷰어의 왼쪽 창에서****Windows 로그 > 시스템** 으로 이동합니다. 오른쪽 창에서 원본값 **MemoryDiagnostics-Results** 가 있는 이벤트를 볼 때까지 **원본** 열을 보며 목록 아래로 검색합니다. 해당되는 각 이벤트를 강조 표시하고 목록 아래의 **일반** 탭 아래에 있는 상자에서 결과 정보를 확인합니다.
