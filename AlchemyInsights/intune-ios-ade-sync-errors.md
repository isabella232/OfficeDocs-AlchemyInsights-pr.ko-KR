---
title: Apple 자동 장치 등록 동기화 오류
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49707892"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Apple 자동 장치 등록 동기화 오류

"오류 상태인 ADE/DEP 토큰이 하나 이상 있는 것으로 감지되었습니다. 영향을 받는 각 토큰에 대해 오류 상태가 확인될 때까지 ADE 기능이 동일하게 작동하지 않습니다."

이 오류는 여러 가지 방법으로 매니페스트될 수 있습니다.

1. 장치가 ABM/ASM에서 Intune으로 동기화되지 않을 수 있습니다.
2. 등록 프로필 할당이 실패할 수 있습니다.
3. 장치가 ADE 등록을 완료하지 못했습니다.

장치 등록> Apple 등록 프로그램 토큰> **Apple** 등록 > 장치 등록에서 Intune 콘솔에 보고된 동기화 오류를 확인하고 다음 설명서를 검토하여 잠재적인 수정을 확인합니다.

[iOS/iPadOS 및 macOS 자동화된 장치 등록 토큰에 대한 ABM/ASM 동기화 오류](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
