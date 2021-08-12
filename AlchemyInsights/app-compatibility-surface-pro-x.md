---
title: Microsoft Surface Pro X와의 앱 호환성
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7009"
- "9003951"
ms.openlocfilehash: 8f353d1337415183db1df168406b33594fb5fdb0aac3f13d0afe3e682fa6e3f3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932031"
---
# <a name="app-compatibility-with-microsoft-surface-pro-x"></a>Microsoft Surface Pro X와의 앱 호환성

응용 프로그램은 Surface Pro X와 같은 장치에서 다르게 실행됩니다. 대부분의 앱은 호환되지만 몇 가지 제한 사항이 있습니다. 다음은 응용 프로그램을 실행하는 동안발생할 수 있는 문제의 목록입니다. 

**드라이버입니다.** 드라이버는 Windows 10 ARM 기반 PC용으로 설계된 경우 작동하게 됩니다. 드라이버가 작동하지 않는 경우 앱 혹은 앱이 실행되는 하드웨어도 작동하지 않습니다. 장치에 대한 추가 지원은 [Windows 10 ARM 기반 PC FAQ](https://support.microsoft.com/windows/windows-10-arm-based-pcs-faq-477f51df-2e3b-f68f-31b0-06f5e4f8ebb5)를 참조하거나 또는 하드웨어 제조업체에 문의하세요.

**64비트(x64) 앱입니다.** 64비트(x64)인 앱은 작동하지 않습니다. 64비트(ARM64) 앱, 32비트(ARM32) 앱 또는 32비트(x86) 앱이 필요합니다. 일반적으로 32비트(x86) 버전의 앱을 찾을 수 있지만 일부 앱 개발자는 64비트(x64) 앱만 제공합니다.

**사용자 지정된 앱입니다.** 보조 기술 또는 클라우드 저장소 앱과 같은 Windows 환경을 사용자 지정하는 앱은 문제가 발생할 수 있습니다. 자세한 내용은 해당 응용 프로그램 제조업체에 문의하세요.

**타사 바이러스 백신 소프트웨어입니다.** 일부 타사 바이러스 백신 소프트웨어를 설치할 수 없습니다. Windows Security를 사용하면 Windows 10 장치의 지원되는 수명 기간 동안 안전하게 유지할 수 있습니다.

**Windows 팩스 및 스캔입니다.** Windows 팩스 및 스캔은 Windows 10 ARM 기반 PC에서는 사용할 수 없습니다.

앱을 설치, 제거 또는 재설치하는 데 문제가 있는 경우 [앱 문제 해결 세부 사항](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-app-install#app-troubleshooting-details)을 참조하세요.

드문 경우를 제외하고 모든 키워드는 AND가 아니라 OR이 되어야 합니다.