---
title: 응용 프로그램이 검색되지 않음 오류 완화
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 34b2024257c88512db170cbb0e672c1628ad8e3935342f87c5032492e1ad0259
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54026120"
---
# <a name="mitigate-the-application-was-not-detected-error"></a>"응용 프로그램이 검색되지 않았습니다" 오류 완화

Intune에서 보고되는 "설치가 완료된 후 응용 프로그램이 검색되지 않았습니다." 앱 설치 오류가 모든 주요 OS 플랫폼(Windows, iOS, Android)에서 발생할 수 있습니다.

이 오류를 발생시키는 가장 일반적인 시나리오는 다음과 같습니다.

- 초기 배포 후 앱이 Intune 외부에서(타사 앱 스토어) 업데이트되었습니다. 예를 들어 Google Chrome과 같은 일부 응용 프로그램이 자동 업데이트될 수 있습니다.
- 사용자가 최초 설치 후 앱을 제거했습니다.

이 문제를 완화하려면 먼저 영향을 받는 장치에 대한 검토를 수행하여 오류가 발생하는 시나리오를 확인합니다.

- 앱이 Intune 외부에서 업데이트된 경우 응용 프로그램 버전을 무시하도록 앱 배포를 설정할 수 있습니다. 설정하려면 **앱 구성 > 앱 정보** 에서 **앱 버전 무시** 를 **예** 로 설정합니다.
- 클라이언트를 대상으로 하는 경우 응용 프로그램을 "필수"로 배포하고 최신 버전을 배포하는 것이 적적할 수 있습니다.
- 또는 iOS 플랫폼에서 새 응용 프로그램 버전이 사용할 수 있게 되는 대로 자동으로 업데이트하도록 구성할 수 있는 Apple Volume Purchase 프로그램에 연결된 **자동 업데이트** 기능을 사용할 수 있습니다.

앱 설치 문제 해결에 대한 자세한 내용은 [앱 설치 문제 해결](https://docs.microsoft.com/intune/troubleshoot-app-install)을 참조하세요.
