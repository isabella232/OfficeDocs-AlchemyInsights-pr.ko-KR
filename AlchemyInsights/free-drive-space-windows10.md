---
title: Windows 10에서 드라이브 공간 절약
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505362"
---
# <a name="free-up-drive-space-in-windows-10"></a>Windows 10에서 드라이브 공간 절약

Windows의 드라이브 공간을 절약하는 두 가지 옵션은 다음과 같습니다.

- Windows 10에서 드라이브 공간을 절약합니다.
- 외부 저장소 장치로 Windows 10 업데이트의 공간을 확장합니다.

디스크 정리를 사용한 후에도 디스크 공간이 여전히 부족한 경우 Temp 폴더가 Microsoft 스토어에서 사용하는 응용 프로그램(.appx) 파일로 빠르게 채워질 수 있습니다. 이 문제를 해결하려면 스토어를 다시 설정하고 스토어 캐시를 지운 다음 Windows 업데이트 문제 해결사 실행합니다. 다음 단계를 진행하기 전에 Microsoft 스토어를 닫아야 합니다.

**1단계: Microsoft 스토어 다시 설정**

**참고** 기본 설정 및 로그인 세부 정보를 포함하여 장치에서 앱 데이터가 영구적으로 삭제됩니다.

1. **시작** > **설정** > **앱** > **앱 및 기능** 을 선택합니다.

1. 앱 목록에서 Microsoft 스토어를 찾아 선택합니다.

1. **고급 옵션을** 선택합니다.

1. 아래로 스크롤하고 **다시 설정** 을 선택한 후 **다시 설정 확인을** 을 선택합니다.

**2단계: Microsoft 스토어 캐시 지우기**

1. Windows 로고 키 + R을 눌러 실행 대화 상자를 열 수 있습니다.

1. wsreset.exe를 입력하고 **확인** 을 선택합니다.

1. 빈 명령 프롬프트 창이 열립니다. 약 10초 후에 창이 닫히고 스토어가 자동으로 열립니다.

**3단계: Windows 업데이트 다시 설정**

1. **시작** > **설정** > **업데이트 및 보안** > **문제해결** 을 선택합니다.

1. 아래로 스크롤하여 목록에서 **Windows 업데이트** 를 선택한 다음, **문제해결사 실행** 을 선택합니다.

1. 컴퓨터를 다시부팅하고 여전히 문제가 발생하는지 확인합니다.

