---
title: 2681 공격 시뮬레이터의 Microsoft 365
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
ms.openlocfilehash: 43f7ae0df98726e61bfe6f93f91909b0bb8a6d19129a99dc027e8b563bc35a6c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57895797"
---
# <a name="attack-simulator-in-microsoft-365"></a>공격 시뮬레이터를 Microsoft 365

- 공격 시뮬레이터가 누락된 경우 공격 시뮬레이터를 사용하려면 **Microsoft Defender for Office 365** 요금제 2 또는 Office 365 Enterprise **필요합니다.** 공격 **시뮬레이터는** Microsoft Defender for Office 365 플랜 1, E3 Office 365 Enterprise 또는 모든 비즈니스용 Microsoft 365 앱 포함되어 있지 않습니다.

- 시뮬레이트된 공격을 시작하려면 전역 관리자 또는 보안 관리자 권한 및 MFA(다단계 인증)가 필요합니다. 공격 시뮬레이터 요구 사항에 대한 자세한 내용은 이 [항목을 참조하세요.](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)

- Brute Force **Password** 공격 시뮬레이션에 대해 알아야 할 중요한 사항:

  - 대상 계정이 MFA를 사용하도록 설정한 경우 암호를 올바르게 추측한 경우 계정이 손상된 것으로 표시되지 않습니다(두 번째 인증 요소가 불완전합니다).

  - 암호 파일은 10MB보다 클 수 없습니다. 한 줄에 하나의 암호를 사용하며 목록의 마지막 암호 다음에 빈 줄(캐리지 리턴)을 포함합니다.

- 스피어 피싱 연결 시뮬레이션에 대해 알아야 할 **중요한** 사항:

  - 기본적으로 피싱 로그인 서버 URL에 대한 사용자 지정 값을 제공할 **수 없습니다.**

  - 받는 사람이 보고서 [](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) 메시지 추가 기능을 사용하여 메시지를 피싱으로 보고하는 경우 시뮬레이트된 공격이기 때문에 메시지에 대한 경고가 수신되지 않을 수 있습니다.

- 보고서: 시뮬레이션된 공격이 완료되면 공격 **세부 정보를** 클릭하여 보고서를 볼 수 있습니다.

- 공격 시뮬레이터의 자세한 지침과 새로운 기능은 에서 [공격 시뮬레이터를 Microsoft 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)
