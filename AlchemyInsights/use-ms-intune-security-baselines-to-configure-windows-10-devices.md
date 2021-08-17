---
title: 보안 Microsoft Intune 사용하여 Windows 10 구성
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: a94c6b72df3874ee80413adac86d60306175734b6ff28b2e015e05eec6f3838b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104350"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>보안 Microsoft Intune 사용하여 Windows 10 구성

Intune 보안 기준은 사용자와 장치를 보호하는 데 도움이 됩니다. 보안 기준은 관련 보안팀에서 권장하는 알려진 설정 및 기본값 그룹을 적용하는 데 사용되는 Windows 설정의 미리 구성된 그룹입니다. Intune에서 보안 기준 프로필을 만들어 여러 장치 구성 프로필로 구성된 서식 파일을 만듭니다.

사용자 또는 장치 그룹에 보안 기준을 배포하면 해당 설정이 사용자 또는 장치 그룹 이상에서 실행되는 Windows 10 적용됩니다. 예를 들어 MDM 보안 기준은 자동으로 (1) 이동식 드라이브에 BitLocker를 활성화하고( 2) 디바이스 잠금을 해제하는 데 암호가 필요하며, (3) 기본 인증을 사용하지 않도록 설정합니다. 환경에 대해 기본값이 작동하지 않는 경우 필요한 설정을 적용하기 위해 기준을 사용자 지정합니다.

보안 기준은 Microsoft 365에서 엔드투엔드 보안 워크플로를 설정하는 데도 도움이 됩니다. 이 경우의 몇 가지 이점은 다음과 같습니다.

- 보안 기준에는 보안에 영향을 주는 설정에 대한 모범 사례와 권장 사항이 포함되어 있습니다. Intune은 그룹 정책에 대한 기준을 만드는 Windows 보안팀과 협력하기 때문에 이 권장 사항은 견고한 지침과 광범위한 환경을 기반으로 합니다.
- Intune을 처음 사용하며 어디에서부터 시작해야 할지 모르겠는 경우 보안 기준을 사용하면 보안 프로필을 빠르게 만들고 배포할 수 있습니다.
- 현재 그룹 정책을 사용하는 경우 관리 목적으로 Intune으로 마이그레이션하는 것이 훨씬 더 쉬워집니다. 이는 Intune에 기본 제공되어 관리에 대한 최신 기능을 포함하기 때문에 보안 기준을 훨씬 더 쉽게 사용할 수 있습니다.

자세한 내용은 보안 [기준 Windows 모바일](https://go.microsoft.com/fwlink/?linkid=2141503) 장치 관리를 [참조하세요.](https://go.microsoft.com/fwlink/?linkid=2141701)