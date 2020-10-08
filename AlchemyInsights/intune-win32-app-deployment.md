---
title: Intune Win32 앱 배포
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
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366527"
---
# <a name="intune-win32-app-deployment"></a>Intune Win32 앱 배포

Microsoft Intune을 사용하면 MSI와 .EXE를 비롯하여(이에 국한되지는 않음) Win32 응용 프로그램을 Windows 10 장치에 배포할 수 있습니다. 사용되는 배포 메커니즘을 사용하려면 대상 장치에 IME(Intune 관리 확장)이 있어야 합니다. Powershell 스크립트나 win32 응용 프로그램 배포를 사용자/장치에 대상 지정하면 IME가 자동으로 설치됩니다.

또한 다음을 포함하는 Win32 앱을 배포하는 데 충족되어야 하는 사전 필수 항목 집합이 있습니다.

- 지원되는 플랫폼: Windows 10 버전 1607 이상(Enterprise, Pro, 및 Education 버전)입니다.
- 지원되는 아키텍처: x86 및 x64입니다.
- 장치 관리: AAD에서 조인하고 자동으로 등록됩니다(하이브리드 도메인 조인과 그룹 정책 자동 등록 포함).
- 응용 프로그램 패키지 형식: [Microsoft Win32 콘텐츠 Prep 도구](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare)로 준비된 .**intunewin** 파일입니다.
- 제한 사항:
    - 최대 크기: 8GB입니다.
    - 지원되지 않는 아키텍처: ARM입니다.

해당 단계와 관련된 정보를 보려면 “[Microsoft Intune에서 Win32 앱의 추가, 할당 및 모니터링](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)” 문서를 참조하세요.

Win32 앱을 포함하여 Windows에서 응용 프로그램 배포 문제 해결에 대한 자세한 내용은 다음 문서에서 검토 가능

- [앱 설치 문제 해결](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [Win32 앱 문제 해결](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)