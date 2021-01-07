---
title: DataProtection - Bitlocker
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
- "1802"
- "9000220"
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768823"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Intune을 사용하여 Bitlocker 암호화 사용

 Intune 끝점 보호 정책을 사용하여 Windows 장치에 대한 Bitlocker 암호화 설정을 구성할 수 있습니다. 자세한 내용은 Intune을 사용하여 디바이스를 보호하는 [Windows 10 이상 설정을 참조하세요.](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)
 
Windows 10을 실행하는 많은 새 장치는 MDM 정책을 적용하지 않고 트리거되는 자동 Bitlocker 암호화를 지원해야 합니다. 기본 설정이 아닌 설정이 구성된 경우 정책 적용에 영향을 줄 수 있습니다. 자세한 내용은 다음 FAQ를 참조합니다.
 
BitLocker 문제 해결에 대한 자세한 내용은 [Microsoft Intune에서 BitLocker 정책 문제 해결을 참조하세요.](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)
 
 
**FAQ**

Q: Endpoint Protection 정책을 사용하여 장치 암호화를 지원하는 Windows 버전은 무엇입니까?<br>
A: Intune 끝점 보호 정책의 설정은 [Bitlocker CSP를 사용하여 구현됩니다.](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp) Windows의 모든 버전 또는 빌드가 Bitlocker CSP를 지원하는 것은 아니며, <br><br>

Q: 최종 사용자 조작 없이 장치에서 Bitlocker를 사용하도록 설정하는 방법<br>
A: 필요한 필수가 충족된 경우 Intune을 통해 Bitlocker "자동 암호화"를 사용하도록 설정할 수 있습니다. 다음 doc에서 자동 암호화를 사용하도록 설정하려면 장치 요구 사항 및 예제 정책 설정에 대한 세부 정보를 [참조하세요. Bitlocker 암호화를 자동으로 사용하도록 설정하십시오.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices) <br><br>

Q: 장치가 암호화 방법 및 암호화 강도(XTS-AES-128)에 대한 OS 기본 설정을 사용하여 Bitlocker로 이미 암호화된 경우 다른 설정으로 정책을 적용하면 새 설정으로 드라이브의 다시 암호화가 자동으로 트리거하나요?<br>
A: 아니요. 새 암호화 설정을 적용하려면 먼저 드라이브의 암호를 해독해야 합니다.<br><br>
**참고:** Autopilot을 사용하여 등록하는 장치의 경우 Intune 정책이 평가될 때까지 OOBE 중에 발생하는 자동 암호화가 트리거되지 않습니다. 그러면 OS 기본값 대신 정책 기반 설정을 사용할 수 있습니다.
 
Q: Intune 정책이 적용된 결과로 장치가 암호화된 경우 해당 정책이 제거될 때 암호가 해독될 수 있나요?<br>
A: 암호화 관련 정책을 제거하면 구성된 드라이브의 암호가 해독되지는 않습니다.
 
Q: Intune 준수 정책에서 장치가 Bitlocker를 사용하도록 설정되지 않은 것으로 표시하는 이유는 무엇입니까?<br>
A: Intune 준수 정책의 "Bitlocker 사용" 설정은 Windows DHA(장치 상태 Attestation) 클라이언트를 사용합니다. 이 클라이언트는 부팅 시 장치 상태만 측정합니다. 따라서 Bitlocker 암호화가 완료된 후 장치를 다시 시작하지 않은 경우 DHA 클라이언트 서비스는 Bitlocker가 활성 상태인 것으로 보고하지 않습니다.
 
 