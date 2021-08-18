---
title: Microsoft Defender for Office 365
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
ms.openlocfilehash: c5043bcd3d40dccc76b348f436001408e42ee7f9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330066"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>Microsoft Defender for Office 365

다음은 Microsoft Defender for Office 365.

- **메시지 지연**:

  전자 메일 배달 지연은 메시지의 첨부 파일 금고 때문에 발생할 수 있습니다. 자세한 내용은 첨부 [파일 금고 설정을 참조하세요.](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings)

- **가극적 또는 부정적 결과** 보고 :

  자세한 내용은 [Microsoft에 메시지와 파일 보고](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft)를 참조하세요.

- **연결 금고 사용**:

  1. 의 Microsoft 365 Defender 포털에서 정책 섹션의 전자 메일 & 공동 작업 정책 & 규칙 위협 <https://security.microsoft.com/>  \>  \> **정책** \> **금고 링크로** 이동하세요. 

     링크 페이지로 직접 금고 **를** <https://security.microsoft.com/safelinksv2> 사용하세요.

  2. 링크 **금고** 페이지에서 정책 이름을 클릭하여 정책을 선택합니다.
  3. 나타나는 세부 정보 플라이아웃에서 다음 단계 중 하나를 수행합니다.
     - 새 정책을 추가하려면 **+ 만들기 를 선택합니다.** 정책 설정을 정의하는 데 도움이 되는 마법사가 실행됩니다.
     - 기존 정책을 편집하려면 정책 이름을 클릭하여 정책을 선택합니다. 세부 정보 플라이아웃이 나타나면  보호 설정 섹션에서 **편집을** 선택합니다.
  4. 보호 **설정 페이지에서** 다음 설정을 구성합니다.
     - 켜기 메시지에서 알 수 없는 잠재적으로 악의적인 **URL에 대한 작업 선택을 켜기.**
     - 조직 **내에서 보낸 메시지에 안전한 링크 적용을 선택합니다.**

  자세한 내용은 [Set up 금고 Links policies in Microsoft Defender for Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies)
