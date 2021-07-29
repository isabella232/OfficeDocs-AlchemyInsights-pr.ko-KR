---
title: 감사 로그에서 메시지 이벤트 삭제 확인
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 7dd9c98bd45c29702fbc6cc14bf82bf7bce7d89d
ms.sourcegitcommit: 89d938a2d402791ae66dddadba3063e9418f48cb
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/28/2021
ms.locfileid: "53630075"
---
# <a name="audit-logs-for-deleted-email-messages"></a>삭제된 전자 메일 메시지에 대한 감사 로그

2019년 1월부터 Microsoft는 기본적으로 사서함 감사 로깅을 켜고 있습니다. 그렇지 않은 경우 특정 사용자에 대한 메시지 삭제 이벤트를 검토하려면 감사에 대한 삭제 작업을 수동으로 사용하도록 설정해야 합니다. 조직 또는 특정 사용자에 대해 사서함 감사 로깅이 이미 사용하도록 설정된 경우 아래 단계를 따릅니다.

1. Microsoft 365 준수 [센터에 로그인합니다.](https://protection.office.com/)

2. 검색 **및 조사를 클릭하고** **감사 로그 검색 을 선택합니다.**

3. 시작 날짜 및  종료 날짜 필드에서 날짜 범위를 **선택합니다.** 조사할 사용자(항목을 삭제한 사용자)의 사용자 이름을 지정합니다. 활동 **필드에서** **지우기** 항목 폴더에서 삭제된 메시지 및 지우기 항목 폴더로 메시지 이동을 **선택합니다.**

4. **검색** 을 클릭합니다.

결과에서 감사 레코드를 선택합니다. 세부 정보 플라이아웃에서 추가 정보를 **클릭합니다.** 삭제된 항목에 대한 추가 정보(예: 제목 줄 및 삭제된 항목의 위치)가 **AffectedItems** 필드에 표시됩니다. **ClientInfoString** 속성은 Outlook, 웹용 Outlook(이전의 Outlook Web App) 또는 기타 장치에서 Outlook Web App 표시됩니다.

자세한 내용은 사서함에 대해 전자 [메일 전달을 설정한 사용자 확인을 참조하세요.](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)

**참고:** 감사 로그 기능을 사용하여 삭제된 항목을 검색할 수 없습니다. 에서 삭제된 메시지를 웹용 Outlook 에서 삭제된 [항목 복구를 Outlook Web App.](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)
