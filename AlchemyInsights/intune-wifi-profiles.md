---
title: Intune Wi-Fi 프로필
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
- "1548"
- "9000076"
ms.openlocfilehash: 5e5258806c8a38965467a8878bc8ac922c2668f21abe3602f479dcdaff8c9b5b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028226"
---
# <a name="intune-wi-fi-profiles"></a>Intune Wi-Fi 프로필

MDM 클라이언트용 Wi-Fi 연결의 성공적인 구현은 회사 Wi-Fi 인프라의 요구 사항을 반영하는 올바르게 배포된 프로필에 따라 다릅니다. 조사 중인 클라이언트 플랫폼의 적절한 설정을 검토하려면 다음을 참조하세요. 

[Microsoft Intune에서 Android를 실행하는 장치의 Wi-Fi 설정 추가](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Android Enterprise 전용 Wi-Fi 설정 및 Microsoft Intune에서 완전히 관리되는 장치 추가](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Microsoft Intune에서 iOS 및 iPadOS 장치용 Wi-Fi 설정 추가](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Intune에서 Windows 10 이상 장치용 Wi-Fi 설정 추가](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Intune에서 Windows 장치용 Wi-Fi 설정 추가](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**일반적인 문제**

**Wi-Fi 프로필에 지정된 배포 인증서에 종속된 Wi-Fi 프로필을 배포하는 중입니다. 그러나 구성 프로필에 오류 상태가 표시됩니다.**

장치에 인증서를 받았는지 확인합니다.

1. Intune에서 **모든 장치** 로 이동하여 장치 > **장치 구성** 을 선택합니다.

2. 모든 예상 프로필이 성공적인 상태로 나열되어 있는지 확인합니다.

3. Android 프로필의 경우 인증서 체인에 중간 인증서가 있는 경우 해당 인증서가 Android 장치에 배포되었는지 확인합니다.

    인증서 상태를 확인하려면 **장치 구성** > **프로필** > **Android 중간 CA** > **속성** > **신뢰하는 인증서** 로 이동합니다.

오류가 계속 발생하는 경우 절차와 문제 해결 섹션을 참조하세요. 자세한 내용은 [Microsoft Intune에서 SCEP 인증서 프로필 문제 해결에 대한 개요](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)를 참조하세요.

**장치에 Wi-Fi 프로필을 배포했습니다. Intune에서 성공적으로 연결되었다고 표시되지만 장치가 Wi-Fi에 연결되지 않습니다.**

성공 상태는 Intune에서 구성 된 대로 프로필을 배포 했다는 것을 의미합니다. 그러나 네트워크 및/또는 인증 요구 사항에 이러한 구성이 맞지 않을 수 있습니다. 연결 시도에 대한 자세한 내용은 (Wi-Fi 액세스 포인트 컨트롤러 및 NPS/Radium 서버에 있는) 인프라 및 인증 서비스 내 로그를 검토하세요. 네트워크 인프라 팀 또는 타사 Wi-Fi 공급 업체와 협력하여 로그를 수집하고 검토해야 할 수 있습니다.