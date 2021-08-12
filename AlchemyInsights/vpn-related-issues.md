---
title: VPN 관련 문제
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 1d9c34350d16d96329d1ed56666119dba0433c93ccb7547da5dba4894531e1b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53970985"
---
# <a name="vpn-related-issues"></a>VPN 관련 문제

MDM 클라이언트용 VPN 연결의 성공적인 구현은 VPN 인프라의 요구 사항을 올바르게 반영하는 배포 된 프로필에 따라 다릅니다. 조사 중인 클라이언트 플랫폼의 적절한 설정은 다음을 참조하세요. 

[Intune을 사용하여 VPN 연결을 추가하기 위해 Windows 10 및 Windows 홀로그램 장치 설정](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[Microsoft Intune에서 iOS 및 iPadOS 장치에 VPN 설정 추가](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Intune에서 VPN을 구성하기 위해 Android 장치 설정](https://docs.microsoft.com/intune/vpn-settings-android)  
[Microsoft Intune에서 macOS 장치에 VPN 설정 추가](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

VPN 프로필에서 인증서 기반 인증을 사용하는 경우 VPN 프로필에 연결 된 루트 인증서와 클라이언트 인증서 프로필이 성공적으로 배포 되었는지 확인합니다.

**일반적인 문제**

**장치에 VPN 프로필을 배포 했습니다. Intune에서 성공적으로 연결 되었다고 표시되지만 장치가 VPN에 연결되지 않습니다.**

성공 상태는 Intune에서 구성 된 대로 프로필을 배포 했다는 것을 의미합니다. 그러나 네트워크 및/또는 인증 요구 사항에 이러한 구성이 맞지 않을 수 있습니다. 연결 시도에 대한 자세한 내용은 VPN 서버와 NPS/Radius 서버에 있는 인프라 및 인증 서비스 로그를 참조하세요. 네트워크 인프라 팀 또는 타사 VPN 공급 업체와 협력하여 로그를 수집하고 검토 해야 할 수 있습니다.

**iOS용사용자 지정 VPN을 구성할 때 앱별 VPN 기능을 사용할 수 없습니다.**

Intune에서 iOS용 앱별 VPN은 현재 앱별 VPN 구성 전에 인증서 필수 구성 요소를 충족해야 하는 특정 공급자 및 파트너에게만 제공됩니다. 자세한 내용은 [Intune에서 iOS/iPadOS 장치의 앱별 VPN 설정](https://docs.microsoft.com/intune/vpn-setting-configure-per-app)을 참조하세요. 

Intune의 모든 VPN 연결 유형에 대한 자세한 내용은 [Intune에서 VPN 서버 연결을 위한 VPN 프로필 만들기](https://docs.microsoft.com/intune/vpn-settings-configure)를 참조하세요.  

**구성 된 도메인에 액세스하는 경우 iOS 온-디맨드 VPN이 트리거하지 않음**

자동 VPN 설정을 테스트 하려면 다음 값을 설정합니다.

다음을 수행하고 싶습니다: **각 연결 시도 평가** 

연결할 것인지 선택합니다: **필요한 경우 연결**

사용자가 이러한 도메인에 액세스 하는 경우: **대상***도메인 이름*

위의 구성이 실패할 경우 다음 요소를 추가 합니다:

이 URL에 연결할 수 없는 경우 강제로 VPN에 연결: **BADURL**