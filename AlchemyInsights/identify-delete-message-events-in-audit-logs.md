---
title: 감사 로그에서 메시지 삭제 이벤트 확인
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
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696519"
---
# <a name="audit-logs-for-deleted-email-messages"></a>삭제 된 전자 메일 메시지에 대 한 감사 로그

2019 년 1 월부터 Microsoft는 기본적으로 사서함 감사 로깅을 설정 하 고 있습니다. 그렇지 않고 특정 사용자에 대 한 메시지 삭제 이벤트를 검토 하려면 감사에 대 한 삭제 작업을 수동으로 사용 하도록 설정 해야 합니다. 조직 또는 특정 사용자에 대해 사서함 감사 로깅이 이미 사용 하도록 설정 된 경우에는 아래 단계를 수행 합니다.

1. [Microsoft 365 보안 & 준수 센터](https://protection.office.com/) 에 로그인 합니다.

2. **검색 및 조사** 를 클릭 하 고 **감사 로그 검색**을 선택 합니다.

3. **시작 날짜** 및 **끝 날짜** 필드에서 날짜 범위를 선택 합니다. 조사 하려는 사용자에 대 한 사용자 이름 (항목을 삭제 한 사용자)을 지정 합니다. **작업** 필드에서 **지운 편지함 폴더에서 삭제 된 메시지** 를 선택 하 고 **메시지를 지운 편지함 폴더로 이동**합니다.

4. **검색**을 클릭합니다.

결과에서 감사 레코드를 선택 합니다. 세부 정보 플라이 아웃에서 **추가 정보**를 클릭 합니다. 삭제 된 항목에 대 한 추가 정보 (예: 제목 줄 및 삭제 시 항목의 위치)가 **AffectedItems** 필드에 표시 됩니다. **Clientinfostring** 속성은 outlook, 웹에서 outlook (이전의 Outlook web App) 또는 다른 모든 장치에서 삭제를 수행 했는지 여부를 표시 합니다.

자세한 내용은 [사서함에 대 한 전자 메일 전달을 설정한 사용자 결정](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)를 참조 하세요.

**참고**: 감사 로그 기능을 사용 하 여 삭제 된 항목을 검색할 수는 없습니다. 웹용 Outlook에서 삭제 된 메시지를 검색 하려면 [Outlook Web App에서 삭제 된 항목 복구](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)를 참조 하세요.
