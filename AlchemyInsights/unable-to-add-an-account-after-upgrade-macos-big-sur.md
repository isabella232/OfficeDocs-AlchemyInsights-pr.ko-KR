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
ms.openlocfilehash: 91cb402e63b68de4a08f6dcb80807ff2e01300c9
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/22/2021
ms.locfileid: "59475129"
---
# <a name="unable-to-add-an-account-after-upgrading-to-macos-116-big-sur"></a>macOS 11.6 Big Sur로 업그레이드한 후 계정을 추가할 수 없음

macOS 11.6으로 업그레이드한 후 회사 또는 학교용 OneDrive 계정 또는 OneDrive 개인 계정이 계정 목록에 표시되지 않을 수 있으며 앱에서 두 번째 계정에 로그인하지 못할 수 있습니다.

이 문제에 대한 수정 사항이 개발되었습니다. 먼저 OneDrive의 독립 실행형 또는 App Store 버전을 실행 중인지 확인합니다.

- 메뉴 모음에서 OneDrive 클라우드 > **도움말 및 설정** > **기본 설정** > **정보** 를 선택합니다. 버전 번호에 **(독립 실행형)** 이 포함되지 않는 경우 제품의 App Store 버전이 있습니다.

독립 실행형 버전의 OneDrive를 사용하는 경우 컴퓨터를 다시 시작하면 OneDrive가 이 문제를 해결한 빌드로 자동 업데이트를 합니다. 빌드를 수동으로 설치하려면 이 [.zip 파일](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip)을 다운로드하여 파일의 압축을 해제하고 (기존 OneDrive 앱을 바꾸어) OneDrive 앱을 응용 프로그램 폴더에 복사합니다.

App Store 버전을 사용하는 경우 독립 실행형 버전의 OneDrive 설치를 고려하세요. 이 버전은 App Store 버전과 동일한 방식으로 작동하지만 Microsoft에서 사용자에게 더 빠르게 업데이트를 제공하고 이 문제에 대한 수정 사항이 포함된 버전에 연결하도록 합니다.

1. [수정 사항이 포함된 독립 실행형 버전의 OneDrive](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip)를 다운로드합니다.
2. 파일 압축을 해제하고 (기존 OneDrive 앱을 바꾸어) OneDrive 앱을 응용 프로그램 폴더에 복사합니다.

App Store 버전을 사용해야 하는 경우 앱 스토어에서 수정 사항이 포함된 앱 버전을 릴리스할 때까지 기다리세요. 유감스럽게도 Microsoft는 App Store에서 최종 버전이 릴리스될 예정일을 알려드릴 수 없습니다.


