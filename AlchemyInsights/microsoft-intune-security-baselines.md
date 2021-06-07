---
title: 보안 Microsoft Intune 사용하여 Windows 10 구성
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783229"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>보안 Microsoft Intune 사용하여 Windows 10 구성

Intune 보안 기준은 사용자와 장치를 보호하는 데 도움이 됩니다. 보안 기준은 Windows 팀에서 권장하는 알려진 설정 및 기본값 그룹을 적용하는 데 사용되는 미리 구성된 그룹에 대한 기본 설정입니다. Intune에서 보안 기준 프로필을 만들어 여러 장치 구성 프로필로 구성된 서식 파일을 만듭니다.

사용자 또는 장치 그룹에 보안 기준을 배포하면 해당 설정이 사용자 또는 장치 그룹 이상에서 실행되는 Windows 10 적용됩니다. 예를 들어 Microsoft MDM(모바일 장치 관리) 보안 기준은 이동식 BitLocker 사용할 수 있는 보안 기준을 자동으로 설정하고, 디바이스 잠금을 해제하는 데 암호가 필요하며, 기본 인증을 사용하지 않도록 설정합니다. 환경에서 기본값이 작동하지 않는 경우 필요한 설정을 적용하기 위해 기준을 사용자 지정할 수 있습니다.

보안 기준은 Microsoft 365에서 엔드투엔드 보안 워크플로를 설정하는 데도 도움이 됩니다. 보안 기준에는 보안에 영향을 주는 설정에 대한 모범 사례와 권장 사항이 포함되어 있습니다. 그룹 정책에 대한 기준을 만드는 Windows 보안 팀과 Intune 파트너가 있으므로 이러한 권장 사항은 견고한 지침과 광범위한 환경을 기반으로 합니다.

Intune을 새로 사용하며 시작할 위치를 알 수 없는 경우 보안 기준을 사용하면 보안 프로필을 빠르게 만들고 배포할 수 있습니다. 현재 그룹 정책을 사용하는 경우 관리 목적으로 Intune으로 마이그레이션하는 것이 Intune에 기본 제공되어 최신 관리 기능을 포함하기 때문에 보안 기준을 훨씬 더 쉽게 사용할 수 있습니다.

자세한 내용은 보안 [기준 Windows 모바일](/windows/security/threat-protection/windows-security-baselines) 장치 관리를 [참조하세요.](/windows/client-management/mdm/)

