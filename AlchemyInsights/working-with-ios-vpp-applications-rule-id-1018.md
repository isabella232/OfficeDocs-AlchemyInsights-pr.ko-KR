---
title: iOS VPP 응용 프로그램 규칙 ID 1018 작업
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: f693d12ff0f9c193cba0c6a6802b22d7acd37532c65986e5f6613e18c021f06b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083020"
---
# <a name="working-with-ios-vpp-applications"></a>iOS VPP 응용 프로그램 작업

Apple 볼륨 구매 프로그램을 사용하여 구입한 iOS 앱을 관리하는 방법을 Microsoft Intune Apple 볼륨 구매 프로그램을 활용하기 위한 [기능,](https://docs.microsoft.com/intune/vpp-apps-ios) 제약 조건 및 단계 및 앱에 대한 지원에 대해 Microsoft Intune.
  
 **일반적인 문제:** "사용자에게 iOS VPP 앱을 할당했지만 설치에 실패했습니다."
  
- 여러 모바일 장치 관리 공급자에서 단일 VPP 토큰을 사용하는 경우 이러한 문제가 발생될 수 있습니다. Apple의 VPP 토큰은 하나의 공급자에서만 사용할 수 있습니다. 여러 공급자와 함께 VPP 토큰을 사용한 경우 토큰을 Intune에 다시 업로드해야 합니다.

- 총 설치 수가 라이선스 수를 초과하면 설치가 실패할 수 있습니다. 라이선스에 대한 사용 현황 보고서를 확인한 후 **Intune 모바일** 앱 앱 라이선스 \> **페이지로 이동합니다.** 사용 중이 있는 라이선스를 취득하는 방법에 대한 자세한 내용은 이 문서를 [참조하세요.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
