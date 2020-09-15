---
title: Yammer 라이브 이벤트 만들기 오류
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002495"
- "5112"
ms.openlocfilehash: 1b342b17e4b91804a75c46352f3ef7d7814bfcee
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47675448"
---
# <a name="live-events-in-yammer-creation-errors"></a>Yammer 라이브 이벤트 만들기 오류

**Yammer 라이브 이벤트 만들기**

Yammer에는 항상 라이브 이벤트를 만들 수 있는 옵션이 표시됩니다. 경우에 따라 사용자가 라이브 이벤트를 만들기를 위한 필수 조건을 충족하지 못하여 만들려고 하면 오류가 발생하는 경우도 있습니다. 아래 항목에서는 이 문제의 일반적인 원인을 다루며 최종 사용자에게 이 문제를 해결하는 방법을 제공합니다.

**라이브 이벤트를 만들 수 있는 사용자**
- Office 365 Enterprise E1, E3 또는 E5 라이선스 또는 Office 365 A3 또는 A5 라이선스.
- Microsoft Teams 관리 센터에서 라이브 이벤트를 만들기 위한 권한.
- Microsoft Stream에서 라이브 이벤트를 만들기 위한 권한(외부 브로드캐스팅 앱 또는 디바이스를 사용하여 생성한 이벤트용).
- 조직의 전체 팀 구성원 자격(게스트 또는 다른 조직의 구성원 자격은 제외).
- 팀 모임 정책에 설정된 비공개 모임 예약, 화면 공유 및 IP 비디오 공유.

**라이브 이벤트 만들기 정책**

Yammer는 스트림의 Office 365 테넌트에 설정된 라이브 이벤트 정책을 따릅니다. 기본적으로 조직의 모든 사용자가 라이브 이벤트를 만들 수 있습니다. 관리자는 [사용자가 라이브 이벤트를 만들지 못하도록 할 수 있는 이 설정을 변경](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating)할 수 있습니다. 사용자에게 정책 오류가 발생하는 경우 라이브 이벤트를 만들 수 있는 권한이 있는지 확인하는 것이 중요합니다.
