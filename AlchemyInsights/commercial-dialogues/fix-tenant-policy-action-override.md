---
title: 테넌트 정책 수정(작업 오버라이드)
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
ms.openlocfilehash: 9c0b88c1ca2120acccd9cd75eb918a81bde52ec3919f6148922f077f07899da7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034940"
---
# <a name="fix-tenant-policy-action-override"></a>테넌트 정책 수정(작업 오버라이드)

테넌트의 스팸 방지 정책이 이 메시지에 영향을 주었다. 정책을 검토하기 위해 다음을 합니다.

1. Office 365 보안 & [센터로](https://go.microsoft.com/fwlink/p/?linkid=2077143)이동한 다음 위협 관리 정책 스팸 방지  >    >  [로 이동 합니다.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. 정책 **원본에** 다음이 나타내는지  **확인: Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC 메시지**

    그렇다면 사용자 지정 **탭에서** 메시지에 영향을 주는 정책의 설정을 확인합니다. 고객이 메시지에 영향을  주면 모든 Exchange Online Protection 표준 설정이 적용될 수 있습니다.

스팸 필터 정책 구성에 대한 자세한 내용은 스팸 필터 정책 [구성을 참조하세요.](https://go.microsoft.com/fwlink/?linkid=2101431)
