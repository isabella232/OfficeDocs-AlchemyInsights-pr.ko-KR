---
title: 야간 표시 설정 도움말
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
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123142"
---
# <a name="help-with-the-night-light-display-setting"></a>야간 표시 설정 도움말

야간 표시 설정에 대한 자세한 내용은 [Windows 10에서 야간 표시 설정](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)을 참조하세요.

설정에서 야간 조명 옵션이 회색으로 표시된 경우 디스플레이 드라이버를 확인하세요. 

1. 작업 표시줄의 검색 상자를 클릭하고 **장치 관리자** 를 입력한 다음 검색 결과에서 **장치 관리자** 를 선택합니다.
1. **어댑터 표시** 를 확장합니다. 

장치가 DisplayLink 드라이버 또는 Basic Display 드라이버를 사용하는 경우에는 야간 조명 기능을 사용할 수 없습니다.

야간 조명 기능은 최신 그래픽 기술을 활용하므로 디스플레이 드라이버를 업데이트해야 할 수 있습니다.  

- **시작** > **설정** > **업데이트 및 보안** > **Windows 업데이트** > **업데이트 확인** 으로 이동하여 업데이트를 확인하세요.  

또는

- 하드웨어 제조업체의 지원 웹 사이트를 방문하여 최신 디스플레이 드라이버를 수동으로 다운로드하고 설치합니다.

## <a name="reset-night-light-in-the-registry"></a>레지스트리의 야간 표시등 다시 설정

디스플레이 드라이버를 업데이트하지 못한 경우 레지스트리에서 야간 조명을 재설정해야 할 수 있습니다.  

**주의:** 이 문제 해결 단계는 고급 사용자에게만 권장됩니다. 레지스트리를 잘못 수정하는 경우 심각한 문제가 발생할 수 있습니다. 추가 보호를 위해 문제가 발생한 경우 복원할 수 있도록 레지스트리를 수정하기 전에 백업하세요.

1. 검색 상자에 **regedit** 을 입력하고 검색 결과에 **레지스트리 편집기** 를 선택합니다.

1. 다음 레지스트리 키로 이동합니다. 

    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount

1. 내보내고 $$windows.data.bluelightreduction.bluelightreductionstate 하위 키를 삭제합니다.

1. 내보내고 $$windows.data.bluelightreduction.settings 하위 키를 삭제합니다.

1. Windows를 다시 시작하고 야간 표시등 옵션을 사용할 수 있는지 여부를 확인합니다.


