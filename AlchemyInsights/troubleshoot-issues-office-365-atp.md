---
title: Office 365 ATP (Advanced Threat Protection) 관련 문제 해결
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 4164781a331ec919811332e94636449e9d88430d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758071"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a>Office 365 ATP 문제 해결

- **전자 메일 메시지 배달이 지연 되는지**여부 ATP 안전한 첨부 파일 정책에 대해 동적 배달 옵션을 사용해 보세요. 이렇게 하면 악성 파일에서 받는 사람을 보호 하는 동안 전자 메일 메시지 배달이 지연 되지 않습니다.
- 가양성 **또는 거짓 네거티브를 보고**하시 겠어요? 이 링크를 사용 하 여 분석을 위해 파일을 제출 합니다. [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)
- **조직의 사용자 간에 전송 되는 전자 메일에 대해 ATP 안전한 링크 보호를 사용 하도록 설정할 수 있는지 확인 해야 합니다**. 다음 단계를 따릅니다.
    1. 으로 이동 하 https://protection.office.com 여 로그인 합니다.
    2. **위협 관리**  >  **정책**  >  **안전한 링크로**이동 합니다.
    3. **특정 받는 사람에 게 적용 되는 정책**아래에서 정책을 편집 (또는 추가) 합니다.
    4. **조직 내에서 보낸 메시지에 안전한 링크 적용을**선택 합니다.
    5. 정책을 저장 하 고 변경 내용이 데이터 센터를 통해 작동 하는 데 30 분 정도 걸릴 수 있습니다.
- ATP에 대 한 자세한 도움말을 보려면 [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp)를 참조 하세요.