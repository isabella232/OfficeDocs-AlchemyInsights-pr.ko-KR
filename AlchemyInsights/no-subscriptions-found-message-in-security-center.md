---
title: 보안 센터에서 구독 메시지를 찾을 수 없습니다.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 24b9a7d3e8106c7357f14a00ecb192af4644257577a9549620b6e8b11b6f90d0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54097456"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>보안 센터에서 구독 메시지를 찾을 수 없습니다.

Microsoft Defender 보안 센터에 액세스하는 동안 "구독을 찾을 수 없음" 메시지가 표시되면 사용자를 포털에 로그인하는 데 사용되는 AAD(Azure Active Directory)에 Microsoft Defender ATP 라이선스가 없음을 의미합니다.  

Windows E5 및 Office E5 라이선스는 별도의 라이선스입니다.

라이선스를 구입했지만 이 AAD 인스턴스에 프로비저닝되지 않은 경우 지원 사례를 엽니다. 다음 중 하나의 문제일 수 있습니다. <br/>
-   라이선스 프로비저닝 문제일 수 있습니다.<br/>
-   서비스 인증에 사용된 것과 다른 라이선스를 Microsoft AAD에 프로비저닝했습니다.