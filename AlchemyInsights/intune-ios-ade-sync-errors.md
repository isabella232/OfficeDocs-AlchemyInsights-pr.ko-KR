---
title: Apple 자동 장치 등록 동기화 오류
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448928"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Apple 자동 장치 등록 동기화 오류

"오류 상태인 ADE/DEP 토큰이 하나 이상 있는 것으로 감지되었습니다. 영향을 받는 각 토큰에 대해 오류 상태가 확인될 때까지 ADE 기능이 예상대로 작동하지 않습니다."

이 오류는 여러 가지 방법으로 매니페스트될 수 있습니다.

1. 장치가 ABM/ASM에서 Intune으로 동기화되지 않을 수 있습니다.
2. 등록 프로필 할당이 실패할 수 있습니다.
3. 장치가 ADE 등록을 완료하지 못했습니다.

장치 등록 > Apple 등록 프로그램 토큰에서 Intune > 보고된 > 동기화 **> 확인합니다.**

동기화 오류의 가장 일반적인 원인 중 하나는 현재 토큰의 만료입니다. 대부분의 경우 영향을 받는 토큰을 갱신하면 문제가 해결됩니다.

하나 이상의 토큰이 만료된 경우 다음 설명서를 참조하여 토큰을 적절하게 갱신할 수 있습니다.

[자동화된 장치 등록 토큰 갱신](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

또한 다음 설명서를 참조하여 토큰 동기화 실패의 원인이 되는 다른 오류에 대한 잠재적인 수정을 볼 수 있습니다.

[iOS/iPadOS 및 macOS 자동화된 장치 등록 토큰에 대한 ABM/ASM 동기화 오류](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[iOS/iPadOS 및 macOS 자동화된 장치 등록 토큰에 대한 ABM/ASM 동기화 오류](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
