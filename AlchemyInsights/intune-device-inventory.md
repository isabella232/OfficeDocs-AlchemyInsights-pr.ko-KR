---
title: Intune 장치 인벤토리
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 00ee4f1d7130c239272e28ee8e051a18e6e0baf13040d2a892866be5900adfaf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54014078"
---
# <a name="intune-device-inventory"></a>Intune 장치 인벤토리

장치 블레이드에서는 장치 단위로 Intune에서 관리 중인 장치에 대한 관리자 인싸이트를 제공합니다. 하드웨어, 검색 된 응용 프로그램, 장치 준수 상태 및 장치 구성 상태 등을 포함한 정보가 보여집니다.

하드웨어 및 검색 된 응용 프로그램 인벤토리 데이터는 7일 주기로 수집됩니다. 보고되는 하드웨어의 응용 프로그램 및 특정 요소는 장치 운영 체제와 장치가 개인용인지 회사용인지 여부에 따라 다릅니다.

자세한 내용은 [Intune에서 장치 자세히 보기](https://docs.microsoft.com/intune/device-inventory)를 참조하세요.

**FAQ**

Q: Intune에 등록 된 Windows 장치에 존재하는 응용 프로그램에 전체 인벤터리 목록을 받고 있지 않습니다. 왜 그런가요?

A:이 경우에는 회사 장치로 식별되는 Windows 10 PC 최신 앱만 나열 됩니다. Intune이 이 장치에 설치 된 Win32 앱 정보를 수집 하지 않습니다.

Q: 모든 장치에서 전화 번호가 수집 되지 않는 이유는 무엇인가요?

A: 예를 들어, 사용자가 모바일 장치 인벤터리 보고서를 실행 할 때 Intune에서 회사 장치로 분류되는 전화의 전체 전화 번호는 식별되지 않습니다. 나만의 장치 전화 번호는 항상 별표 (****)로 부분적으로 마스킹 하고 마지막 네 자릿수만 표시합니다.