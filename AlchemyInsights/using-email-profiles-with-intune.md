---
title: Intune에서 전자 메일 프로필 사용
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
- "1559"
- "9000076"
ms.openlocfilehash: b1653b73e7296e7eed411ae73c19342a1187b2eb7e287cff4339ea0ca32d75c1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919429"
---
# <a name="using-email-profiles-with-intune"></a>Intune에서 전자 메일 프로필 사용

Intune을 사용하여 기본(기본 제공) 전자 메일 클라이언트의 전자 메일 프로필을 만들고 여러 장치 플랫폼에 배포할 수 있습니다.

기존 프로필이 처리되는 방식과 전자 메일 프로필을 제거하는 방법을 비롯하여 전자 메일 프로필과 관련된 일부 제한 사항에 대한 자세한 내용은 [Intune을 사용하여 장치에 전자 메일 설정 추가](https://docs.microsoft.com/intune/email-settings-configure)를 참조하세요.

각 장치 플랫폼의 전자 메일 프로필을 만드는 방법에 대한 자세한 내용은 다음을 참조하세요.

[Android 장치 설정을 사용하여 Intune에서 전자 메일, 인증 및 동기화 구성](https://docs.microsoft.com/intune/email-settings-android)  
[Microsoft Intune에서 iOS 및 iPadOS 장치의 전자 메일 설정 추가](https://docs.microsoft.com/intune/email-settings-ios)  
[Windows Phone 8.1을 실행하는 장치에 대한 Microsoft Intune의 전자 메일 프로필 설정](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Microsoft Intune에서 Windows 10을 실행하는 장치의 전자 메일 프로필 설정](https://docs.microsoft.com/intune/email-settings-windows-10)

**일반적인 동기화 문제**

**Android 전자 메일 프로필의 KNOX를 사용하면 사용자 연락처, 일정 및 작업이 사용자 장치와 동기화되지 않습니다.**

Android KNOX 전자 메일 프로필을 사용하면 관리자가 각 항목을 활성화하여 장치와 동기화할 콘텐츠 형식을 결정할 수 있습니다.

콘텐츠 형식에 대한 설정이 **구성되지 않음**(기본값)으로 설정된 경우, 해당 콘텐츠 형식은 자동으로 동기화되지 않습니다. 사용자가 수동으로 장치에서 원하는 콘텐츠 형식을 직접 활성화할 수 있지만, Intune 정책 설정이 해당 구성을 덮어쓰고 해당 콘텐츠 형식에 대한 동기화가 중지됩니다.

