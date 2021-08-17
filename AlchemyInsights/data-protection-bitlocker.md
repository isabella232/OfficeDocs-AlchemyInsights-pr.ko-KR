---
title: DataProtection - Bitlocker
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
- "1802"
- "9000220"
ms.openlocfilehash: 3f6e48b9d2f7562d74d60c2901759a7ab359e5c67bd4aa2d556d941a41ab680c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118600"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Intune을 사용하여 Bitlocker 암호화 사용

Intune Endpoint Protection 정책을 사용하여 장치용 Bitlocker 암호화 설정을 구성할 Windows 있습니다. 자세한 내용은 [Intune을 Windows 10](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)보호하는 설정 및 이후 설정을 참조하세요.

Endpoint Protection 정책 외에도 디바이스의 암호화 상태에 대한 자세한 보기를 제공하는 암호화 보고서도 있습니다. 이 보고서는 장치 및 모니터링의 MEM **포털에서**> 다음 구성 **선택** 암호화 [보고서에서 액세스할 수 있습니다.](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport)

Bitlocker를 예상대로 사용하도록 설정하지 못하거나 Bitlocker를 사용하도록 설정하는 데 사용되는 프로필이 오류 상태인 경우 암호화 보고서를 검토하여 동작이 발생하는 이유를 더 잘 이해하세요.

다양한 암호화 상태 값을 포함하여 보고서를 해석하는 방법에 대한 자세한 내용은 Intune을 사용하여 장치 암호화 [모니터링을 참조하세요.](https://docs.microsoft.com/mem/intune/protect/encryption-monitor)

MDM 정책을 적용하지 않고 트리거되는 자동 Bitlocker Windows 10 실행하는 많은 새 디바이스가 지원됩니다. 기본 설정이 아닌 설정이 구성된 경우 정책 적용에 영향을 줄 수 있습니다. 자세한 내용은 다음 FAQ를 참조합니다.

BitLocker 문제 해결에 대한 자세한 내용은 [에서 BitLocker 정책 문제 해결을 Microsoft Intune.](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)
 
 
**FAQ**

Q: Windows 정책을 사용하여 장치 암호화를 지원하는 Endpoint Protection 버전은 무엇입니까?<br>
A: Intune Endpoint Protection 정책의 설정은 [Bitlocker CSP를 사용하여 구현됩니다.](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp) 모든 버전 또는 빌드의 Windows Bitlocker CSP를 지원하지는 않습니다. <br><br>

Q: 최종 사용자 조작 없이 장치에서 Bitlocker를 사용하도록 설정하는 방법<br>
A: 필요한 필수가 충족된 경우 Intune을 통해 Bitlocker "자동 암호화"를 사용하도록 설정할 수 있습니다. 다음의 doc: [Silently Enable Bitlocker Encryption에서](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices)자동 암호화를 사용하도록 설정하려면 장치 요구 사항 및 예제 정책 설정에 대한 세부 정보를 참조하세요. <br><br>

Q: 장치가 암호화 방법 및 암호화 강도에 대한 OS 기본 설정(XTS-AES-128)을 사용하여 이미 Bitlocker로 암호화된 경우 다른 설정을 사용하는 정책을 적용하면 새 설정으로 드라이브의 다시 암호화가 자동으로 트리거하나요?<br>
대답: 아니요. 새 암호화 설정을 적용하려면 먼저 드라이브의 암호를 해독해야 합니다.<br><br>
**참고:** Autopilot을 사용하여 등록하는 장치의 경우 Intune 정책이 평가될 때까지 OOBE 중에 발생하는 자동 암호화가 트리거되지 않습니다. 이렇게 하면 OS 기본값 대신 정책 기반 설정을 사용할 수 있습니다.
 
Q: Intune 정책이 적용된 결과로 장치가 암호화된 경우 해당 정책이 제거될 때 암호가 해독될 수 있나요?<br>
A: 암호화 관련 정책을 제거하면 구성된 드라이브의 암호 해독이 되지 않습니다.
 
Q: Intune 규정 준수 정책은 장치가 Bitlocker를 사용하도록 설정되어 있지 않은 것으로 표시하는 이유는 무엇입니까?<br>
A: Intune 준수 정책의 "Bitlocker 사용" 설정은 DHA(장치 상태 Windows) 클라이언트를 사용합니다. 이 클라이언트는 부팅 시 장치 상태만 측정합니다. 따라서 Bitlocker 암호화가 완료된 후 장치를 다시 시작하지 않은 경우 DHA 클라이언트 서비스는 Bitlocker가 활성 상태인 것으로 보고하지 않습니다.
 
 