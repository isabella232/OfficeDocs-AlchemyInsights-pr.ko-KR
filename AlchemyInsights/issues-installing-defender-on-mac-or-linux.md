---
title: Mac 또는 Linux에 Microsoft Defender를 설치하는 문제
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 39f180852fd0438597fa1ce665b2703fbc7b1aa4
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539686"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Mac 또는 Linux에 Microsoft Defender를 설치하는 문제

**Mac**

- Mac용 Microsoft Defender ATP를 설치하기 전에 시스템 요구 사항이 충족되었는지 확인합니다. 자세한 내용은 [Mac용 Microsoft Defender ATP 설치 방법](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)을 참조하세요.  
- "/Library/Logs/Microsoft/mdatp/install.log" 파일에서 정보를 확인합니다.

**Linux**

- Linux용 Microsoft Defender ATP를 설치하기 전에 시스템 요구 사항이 충족되었는지 확인합니다. 자세한 내용은 [Linux용 MDATP 설치 방법](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)을 참조하세요. 
- MDATP 서비스가 실행중인지 확인하려면 [설치 실패](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)를 참조하세요.  
    서비스가 실행되고 있지 않은 경우 문제를 해결하고 문제를 해결하려면 [mdatp 서비스가 실행되고 있지 않은 경우 문제 해결 단계](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)를 참조하세요.
- 제품의 상태를 확인하는 클라이언트 구성을 확인하고 EICAR 텍스트 파일에서 탐지 테스트를 실행하는 단계는 [클라이언트 구성](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration)을 참조하세요.  

    **참고** 액세스 작업에 지원되는 파일 시스템 목록은 [ Linux용 Microsoft Defender ATP](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)를 참조하세요.