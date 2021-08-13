---
title: Microsoft Intune 보안 기준을 사용하여 Windows 10 장치 구성하기
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: 3bb93c196dd4717f5ec297e63284c5bc2840dcf5965cd000f336fde1e982a061
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971525"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a>Windows 10 장치 구성에 Microsoft Intune 보안 기준 사용하기

Intune 보안 기준은 사용자와 장치를 보호하는 데 도움이 됩니다. 보안 기준은 관련 보안팀에서 권장하는 알려진 설정 및 기본값 그룹을 적용하는 데 사용되는 Windows 설정의 미리 구성된 그룹입니다. Intune에서 보안 기준 프로필을 만들어 여러 장치 구성 프로필로 구성된 서식 파일을 만듭니다.

사용자나 장치 그룹에 보안 기준을 배포하면 Windows 10 이상 버전에서 실행되는 장치에 설정이 적용됩니다. 예를 들어 Microsoft MDM(모바일 장치 관리) 보안 기준은 자동으로 (1) 이동식 드라이브에 BitLocker를 활성화하며, (2) 장치 잠금 해제에 암호를 요구하고, (3) 기본 인증을 비활성화합니다. 환경에서 기본값이 작동하지 않는 경우 필요한 설정을 적용하기 위해 기준을 사용자 지정할 수 있습니다.

보안 기준은 Microsoft 365에서 엔드투엔드 보안 워크플로를 설정하는 데도 도움이 됩니다. 다음은 이 기능의 몇 가지 이점입니다.
- 보안 기준에는 보안에 영향을 주는 설정에 대한 모범 사례와 권장 사항이 포함되어 있습니다. Intune은 그룹 정책에 대한 기준을 만드는 Windows 보안팀과 협력하기 때문에 이 권장 사항은 견고한 지침과 광범위한 환경을 기반으로 합니다.
- Intune을 처음 사용하며 어디에서부터 시작해야 할지 모르겠는 경우 보안 기준을 사용하면 보안 프로필을 빠르게 만들고 배포할 수 있습니다.
- 현재 그룹 정책을 사용하고 있는 경우 이러한 보안 기준은 Intune에 기본 제공되며 관리용 최첨단 기능을 포함하기 때문에 보안 기준을 사용하여 관리 목적으로 Intune으로 마이그레이션하는 것이 훨씬 쉽습니다.

자세한 내용은 [Windows 보안 기준](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) 및 [모바일 장치 관리](https://docs.microsoft.com/windows/client-management/mdm/)를 참조하세요.