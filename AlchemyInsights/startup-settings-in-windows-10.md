---
title: Windows 10의 시작 설정
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828158"
---
# <a name="startup-settings-in-windows-10"></a>Windows 10의 시작 설정

**시작할 때 자동으로 실행되는 앱 변경**

1. 시작 [> 앱 > 로 이동합니다.](ms-settings:startupapps?activationSource=GetHelp)

2. 시작 시 실행할 앱이 켜져 있는지 **확인**

**시작할 때 자동으로 실행될 앱 추가**

1. 시작을 **클릭하거나 탭하고** 시작할 때 실행할 앱을 찾아 찾습니다.

2. 앱을 마우스 오른쪽 단추로 클릭하고 추가 를 **클릭한** 다음 파일 위치 **열기 를 클릭합니다.** 그러면 앱 바로 가기가 저장되는 위치가 열립니다. 파일 위치 열기 옵션이 없는 경우 시작 시 앱을 실행할 수 없음을 의미합니다.

3. 파일 위치가 열리면 Windows 로고 키 **+ R을** 누르고 **shell:startup을** 입력한 다음 확인을 **클릭합니다.** 그러면 시작 폴더가 열립니다.

4. 파일 위치에서 시작 폴더로 바로 가기를 복사하여 앱에 붙여넣습니다.

**고급 시작 옵션(안전 모드, UEFI 설정 및 다른 장치에서 부팅 포함)**

1. 이러한 단계는 PC를 다시 시작하기 때문에 작업을 저장하고 열려 있는 문서를 닫습니다.

2. 설정 > [업데이트 & 복구로 > 이동합니다.](ms-settings:recovery?activationSource=GetHelp)

3. 고급 **시작에서** 지금 **다시 시작을 클릭합니다.** 

4. PC가 다시 시작된 후 옵션 선택 화면으로 다음을 실행합니다.

    - USB 드라이브와 같은 장치에서 부팅하려면 장치 **사용을 클릭합니다.**

    - UEFI 설정(BIOS 설정이라고도 하는)을 입력하려면 **UEFI** 펌웨어 > 고급 옵션 > 클릭합니다. 

    - 안전 모드를 입력하거나 고급 시작 설정을 변경하려면 시작 > 고급 옵션 > 문제 해결을 클릭한 다음 다시 **시작을** **클릭합니다.** [BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)복구 키를 입력해야 할 수 있습니다. PC를 다시 시작한 후 사용할 시작 설정을 클릭합니다.