---
title: Windows 10의 시작 설정
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751141"
---
# <a name="startup-settings-in-windows-10"></a>Windows 10의 시작 설정

**시작할 때 자동으로 실행 되는 앱 변경**

1. [시작 > 설정 > 앱](ms-settings:startupapps?activationSource=GetHelp)으로 이동 합니다.

2. 시작할 때 실행 하려는 앱 **이 켜져 있는지 확인 합니다.**

**시작할 때 자동으로 실행할 앱 추가**

1. **시작** 을 클릭 하거나 탭 하 여 시작할 때 실행 하려는 앱을 찾습니다.

2. 앱을 마우스 오른쪽 단추로 클릭 하 고 **자세히**를 클릭 한 다음 **파일 위치 열기**를 클릭 합니다. 이렇게 하면 앱 바로 가기가 저장 되는 위치가 열립니다. 열린 파일 위치에 대 한 옵션이 없는 경우에는 시작할 때 앱이 실행 될 수 없음을 의미 합니다.

3. 파일 위치를 열고 **Windows 로고 키 + R**을 누르고 **shell: startup**을 입력 한 다음 **확인**을 클릭 합니다. 시작 폴더를 엽니다.

4. 파일 위치에서 시작 폴더에 앱의 바로 가기를 복사 하 여 붙여 넣습니다.

**고급 시작 옵션 (안전 모드, UEFI 설정 및 다른 장치에서 부팅 포함)**

1. 이 단계는 PC를 다시 시작 하므로 작업을 저장 하 고 열려 있는 문서를 모두 닫습니다.

2. [& 보안 > 복구를 업데이트 > 설정](ms-settings:recovery?activationSource=GetHelp)으로 이동 합니다.

3. **고급 시작**에서 **지금 다시 시작**을 클릭 합니다. 

4. PC를 다시 시작한 후 옵션 선택 화면에서 다음을 수행 합니다.

    - USB 드라이브와 같은 장치에서 부팅 하려면 **장치 사용**을 클릭 합니다.

    - UEFI 설정 (BIOS 설정)을 입력 하려면 **Uefi 펌웨어 설정 > > 고급 옵션 문제 해결**을 클릭 합니다. 

    - 안전 모드를 시작 하거나 고급 시작 설정을 변경 하려면 **문제 해결 > 고급 옵션 > 시작**을 클릭 한 다음 **다시 시작**을 클릭 합니다. [BitLocker 복구 키](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)를 입력 하 라는 메시지가 표시 될 수 있습니다. PC가 다시 시작 되 면 사용 하려는 시작 설정을 클릭 합니다.