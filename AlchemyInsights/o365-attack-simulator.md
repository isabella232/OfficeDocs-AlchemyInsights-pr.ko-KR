---
title: 2681 Microsoft 365의 공격 시뮬레이터
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 7b48abea3400e3565f2ba33c97e24e5b9923eb3b
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801557"
---
# <a name="attack-simulator-in-microsoft-365"></a>Microsoft 365의 공격 시뮬레이터

- 공격 시뮬레이터가 누락 되었습니까? Attack 시뮬레이터 **에는 Microsoft Defender For Office 365 계획 2 (ATP 계획 2)** 또는 **Office 365 Enterprise E5** 가 필요 합니다. Attack 시뮬레이터는 Microsoft Defender for Office 365 계획 1 (ATP 계획 1), Office 365 Enterprise E3 또는 기타 Microsoft 365 앱 구독에 포함 되어 **있지** 않습니다.

- 시뮬레이트된 공격을 시작 하는 데 사용 하는 계정에는 전역 관리자 또는 보안 관리자 권한 및 MFA (multi-factor authentication)가 필요 합니다. 공격 시뮬레이터 요구 사항에 대 한 자세한 내용은 [이 항목](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)을 참조 하십시오.

- **무작위 암호** 공격 시뮬레이션에 대해 알아야 할 중요 한 사항은 다음과 같습니다.

  - 대상 계정에 MFA를 사용 하 고 암호가 올바르게 추측 되 면 해당 계정에 손상 된 것으로 표시 되지 않습니다 (두 번째 인증 요인은 불완전 함).

  - 암호 파일의 크기는 10mb를 넘을 수 없습니다. 한 줄에 하나씩 암호를 사용 하 고 목록의 마지막 암호 다음에 빈 줄 (캐리지 리턴)을 포함 합니다.

- **스피어 피싱** 연결 시뮬레이션에 대해 알아야 할 중요 한 사항은 다음과 같습니다.

  - 기본적으로 **피싱 로그인 서버 URL** 에는 사용자 지정 값을 제공할 수 없습니다.

  - 받는 사람이 [보고서 메시지 추가 기능을 사용](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) 하 여 피싱로 메시지를 보고 하는 경우 시뮬레이트된 공격 이므로 메시지에 대 한 알림을 받지 못할 수 있습니다.

- 보고서: 시뮬레이트된 공격이 완료 되 면 **공격 세부 정보** 를 클릭 하 여 보고서를 볼 수 있습니다.

- 자세한 지침 및 Attack 시뮬레이터의 새로운 기능은 [Microsoft 365의 Attack 시뮬레이터](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)를 참조 하세요.
