---
title: 응용 프로그램 보호 정책
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: ab6ad9c4bf95ee013c66384ec8449ceb1b56e8f3ea9e95c695dbbab0e9fa3fc3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53969977"
---
# <a name="application-protection-policy"></a>응용 프로그램 보호 정책

APP(Application protection policy)에 처음이라면 [앱 보호 정책 개요](https://docs.microsoft.com/intune/apps/app-protection-policy)를 확인하세요.

APP 사용을 시작하려면 [앱 보호 정책 만들고 할당하는 방법](https://docs.microsoft.com/intune/app-protection-policies)을 참조하세요.

응용 프로그램 보호 정책 요구사항:

- 사용자가 Intune 또는 EMS 라이선스가 있습니다.
- 사용자가 응용 프로그램 보호 정책의 대상이 되는 그룹에 속해 있습니다.
- 장치에서 보호되는 앱에 한 회사의 사용자만 로그인 되어 있습니다.
- 응용 프로그램에서 [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started)을 구현 했습니다. SDK를 지원하는 앱 목록은 [Microsoft Intune 보호 앱](https://docs.microsoft.com/intune/apps-supported-intune-apps)를 참조하세요.

위의 요구 사항을 충족 하는 사용자가 Intune SDK를 사용 하는 앱에 로그인 하면 정책이 적용됩니다. 정책이 적용 되는지 확인 하는 가장 쉬운 방법은 사용자가 정책에서 PIN을 설정 하도록 요청 하는 것입니다. 

자세한 내용은 다음을 참조하세요.

[APP/MAM 문제 해결 FAQ](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[앱 보호 정책 설정의 유효성을 검사 하는 방법](https://docs.microsoft.com/intune/app-protection-policies-validate)

[앱 보호 정책에 전달 시간 이해](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[앱 보호 정책을 모니터링 하는 방법](https://docs.microsoft.com/intune/app-protection-policies-monitor)