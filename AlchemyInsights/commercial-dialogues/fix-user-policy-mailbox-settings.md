---
title: 사용자 정책/사서함 설정 수정
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: fecc52bea66e0aed709a8995d2509f4432c09482459aa575d29e4c7551375211
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034724"
---
# <a name="fix-user-policymailbox-settings"></a>사용자 정책/사서함 설정 수정

사서함의 정크 메일 설정이 이 메시지에 영향을 주었다. 설정을 검토하려면 다음을 합니다.

1. 관리 Exchange 실행합니다. 자세한 내용은 [Open the Exchange Management Shell 을 참조하십시오.](https://go.microsoft.com/fwlink/?linkid=2101432)
2. 다음 명령을 실행합니다(사용자의 전자 메일 주소 사용):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. 보낸 사람 전자 메일 주소가 **TrustedSendersAndDomains** 또는 **BlockedSendersAndDomains의 일부인지 확인** 전자 메일 주소가 목록 중 하나에 있는 경우 해당 주소를 제거해야 할 수 있습니다. 자세한 내용은 [Set-MailboxJunkEmailConfiguration을 참조합니다.](https://go.microsoft.com/fwlink/?linkid=2101047)
