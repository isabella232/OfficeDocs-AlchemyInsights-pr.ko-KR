---
title: macOS 11.6 Big Sur로 업그레이드한 후 계정을 추가할 수 없음
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13840"
- "9008627"
ms.openlocfilehash: a8176de71a1f67004e790a3a98943402a240f656
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446745"
---
# <a name="unable-to-add-an-account-after-upgrading-to-macos-116-big-sur"></a>macOS 11.6 Big Sur로 업그레이드한 후 계정을 추가할 수 없음

macOS 11.6으로 업그레이드한 후 회사 또는 학교용 OneDrive 계정 또는 OneDrive 개인 계정이 계정 목록에 표시되지 않을 수 있으며 앱에서 두 번째 계정에 로그인하지 못할 수 있습니다.

macOS 11.6 업그레이드와 관련된 새로운 문제입니다. 문제가 해결될 때까지 웹 또는 모바일 장치에서 OneDrive 콘텐츠에 액세스할 수 있습니다. Microsoft는 OneDrive 기능을 복원하기 위해 Apple과 협력하고 있습니다.

터미널을 사용하여 누락된 OneDrive 인스턴스를 수동으로 시작할 수도 있습니다. 

**참고**: 이 해결 방법은 (컴퓨터 다시 부팅 또는 OneDrive 앱 업데이트)로 OneDrive가 다시 시작될 때까지만 작동합니다.

누락된 인스턴스가 개인 계정인 경우 터미널을 열고 다음을 입력합니다.

`open "/Applications/OneDrive.app" --new --args /client=Personal`

누락된 인스턴스가 회사 또는 학교 계정인 경우 터미널을 열고 다음을 입력합니다.

`open "/Applications/OneDrive.app" --new --args /client=Business1`

