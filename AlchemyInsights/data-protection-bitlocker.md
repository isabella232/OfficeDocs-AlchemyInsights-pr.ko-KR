---
title: DataProtection-Bitlocker
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
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731245"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Intune을 사용 하 여 Bitlocker 암호화 사용

 Intune Endpoint Protection 정책은 Windows 장치에 대 한 Bitlocker 암호화 설정을 구성 하는 데 사용할 수 있습니다. 자세한 내용은 [Intune을 사용 하 여 장치를 보호 하기 위해 Windows 10 이상 설정을](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)참조 하세요.
 
Windows 10을 실행 하는 많은 최신 장치는 MDM 정책 응용 프로그램 없이 트리거되는 자동 Bitlocker 암호화를 지원 한다는 점을 알고 있어야 합니다. 기본 설정이 아닌 설정을 구성 하면 정책 응용 프로그램에 영향을 줄 수 있습니다. 자세한 내용은 다음 FAQ를 참조 하세요.
 
Bitlocker 문제를 해결 하는 방법에 대 한 자세한 내용은 [Microsoft Intune에서 bitlocker 정책 문제 해결](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)을 참조 하세요.
 
 
**FAQ**

 Q: Endpoint Protection 정책을 사용 하 여 장치 암호화를 지 원하는 Windows 버전은 무엇입니까?<br>
 A: Intune Endpoint Protection 정책의 설정은 [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)를 사용 하 여 구현 됩니다. Windows의 일부 버전 또는 빌드에서는 Bitlocker CSP를 지원 하지 않습니다. <br><br>
      현재는 엔터프라이즈, 교육, 모바일, 모바일 Enterprise 및 Professional (빌드 1809 이상)과 같은 Windows 버전이 지원 됩니다.
 
Q: 암호화 방법 및 암호화 수준 (XTS-128)에 대 한 운영 체제 기본 설정을 사용 하 여 장치가 이미 Bitlocker로 암호화 된 경우 다른 설정의 정책을 적용 하는 경우 새 설정으로 드라이브의 암호화를 자동으로 트리거합니다?<br>
A: 아니요. 새 암호화 설정을 적용 하려면 먼저 드라이브의 암호를 해독 해야 합니다.<br><br>
**참고:** Autopilot을 사용 하 여 등록 되는 장치의 경우, OOBE 중에 발생 하는 자동 암호화는 Intune 정책을 평가할 때까지 트리거되지 않으므로 운영 체제 기본값 대신 정책 기반 설정을 사용할 수 있습니다.
 
Q: Intune 정책 응용 프로그램의 결과로 장치가 암호화 되 면 해당 정책이 제거 될 때 암호가 해독 됩니까?<br>
A: 암호화 관련 정책을 제거 해도 구성 된 드라이브의 암호 해독이 발생 하지 않습니다.
 
Q: Intune 준수 정책에서 Bitlocker가 사용 하도록 설정 되어 있지 않은 경우에도 디바이스에서이를 표시 하는 이유는 무엇 인가요?<br>
A: Intune 준수 정책에서 "Bitlocker enabled" 설정은 DHA (Windows 디바이스 상태 증명) 클라이언트를 사용 합니다. 이 클라이언트는 부팅 시에만 장치 상태를 측정 합니다. 따라서 Bitlocker 암호화를 완료 한 후 장치를 다시 부팅 하지 않으면 DHA 클라이언트 서비스가 Bitlocker가 활성 상태인 것으로 보고 하지 않습니다.
 
 