---
title: 온라인 용어 저장소에서 SharePoint 누락된 용어
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: d99458d6f9b65e44ad5945c909b9a8861cf0b1f23463fcdfd5b8351b1c08d670
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54106432"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Intune을 사용하여 Bitlocker 암호화 사용

Intune Endpoint Protection 정책을 사용하여 Intune을 사용하여 장치를 보호하기 위한 windows10 이상 설정에 설명된 Windows 장치에 대한 Boitlocker 암호화 설정을 구성할 수 있습니다.

MDM 정책을 적용하지 않고 트리거되는 자동 Windows 10 실행하는 많은 새로운 장치가 지원됩니다. 기본 설정이 아닌 설정이 구성된 경우 정책 적용에 영향을 줄 수 있습니다. 자세한 내용은 FAQ를 참조합니다.


FAQ Q: Windows 정책을 사용하여 장치 암호화를 지원하는 Endpoint Protection 버전은 무엇입니까?
A: Intune Endpoint Protection 정책의 설정은 Bitlocker CSP를 사용하여 구현됩니다.  모든 버전 및 빌드의 Windows Bitlocker CSP를 지원하지는 않습니다. 현재 Windows 버전: Enterprise; 교육, 모바일, 모바일 Enterprise Professional(빌드 1809 이상)가 지원됩니다.




Q: 장치가 암호화 방법 및 암호화 강도에 대한 OS 기본 설정을 사용하여 Bitlocker로 이미 암호화된 경우(XTS-AES-128) 다른 설정을 사용하여 정책을 적용하면 새 설정으로 드라이브의 다시 암호화가 자동으로 트리거하나요?

대답: 아니요. 새 암호화 설정을 적용하려면 먼저 드라이브의 암호를 해독해야 합니다.

참고 Autopilot을 사용하여 등록하는 장치의 경우 Intune 정책이 평가될 때까지 OOBE 중에 발생하는 자동 암호화가 트리거되지 않습니다. 이 경우 OS 기본값 대신 정책 기반 설정을 사용할 수 있습니다.




Q Intune 정책이 적용된 결과로 장치가 암호화된 경우 해당 정책을 제거할 때 암호가 해독될 것인가?

A: 암호화 관련 정책을 제거하면 구성된 드라이브의 암호 해독이 되지 않습니다.




Q: Intune 준수 정책에 내 장치에 "Bitlocker 사용"이 없지만 표시되어 있는 이유는 무엇입니까?

A: intune 규정 준수 정책의 "Bitlocker 사용" 설정은 Windows DHA(장치 상태 Windows) 클라이언트를 사용합니다. 이 클라이언트는 부팅 시 장치 상태만 측정합니다. 따라서 bitlocker 암호화가 완료된 후 장치를 다시 시작하지 않은 경우 DHA 클라이언트 서비스는 bitlocker가 활성 상태인 것으로 보고하지 않습니다.