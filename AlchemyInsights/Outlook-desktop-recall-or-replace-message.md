---
title: Outlook 데스크톱 전자 메일 메시지 회수 또는 교체
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663996"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Outlook 전자 메일 메시지 회수 또는 교체

- 관리자는 **PowerShell을 사용 하 여 사용자를 대신 하 여 메시지를 회수할**수 있습니다. 관리 센터에서 메시지를 회수할 수 없습니다.
- **조직의 사용자에 게 전송 된 메시지만 회수할**수 있습니다. 예를 들어, 메시지가 Gmail 주소로 전송 된 경우에는 회수할 수 없습니다.
- **PC에서 Outlook 2016에서 보낸 메시지만 회수할**수 있습니다. 사용자가 Outlook for Mac 또는 웹용 Outlook을 사용 하 여 메시지를 보낼 경우에는 회수할 수 없습니다.

전자 메일 메시지를 회수 하거나 교체 하려면:

1. Outlook 창 왼쪽의 폴더 창에서 보낸 편지함 폴더를 선택 합니다.
1. 회수 하려는 메시지를 두 번 클릭 하 여 엽니다.
1. **메시지** 탭을 선택 하 고 **작업**  >  **회수 메시지**를 선택 합니다.
1. **이 메시지의 읽지 않은 복사본 삭제** 또는 **읽지 않은 복사본 삭제**를 선택 하 고 새 메시지로 바꾼 후 **확인**을 선택 합니다.
1. 대체 메시지를 보내는 경우 메시지를 작성 한 다음 **보내기를**선택 합니다.
1. 메시지 회수의 성공 또는 실패는 Outlook의 받는 사람 설정에 따라 달라 집니다. 회수를 확인 하는 단계는 [이 문서](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)를 참조 하십시오.

조직의 전자 메일 메시지 검색 및 삭제하기

- 전역 관리자가 아닌 경우 메시지를 검색 하려면 eDiscovery 관리자 역할 또는 준수 검색 관리 역할에 계정을 추가 해야 합니다. 메시지를 삭제 하려면 조직 관리 역할 그룹 또는 검색 및 삭제 관리 역할에 참가 해야 합니다. 이러한 역할에 대 한 사용 권한은 [보안 및 준수 센터](https://go.microsoft.com/fwlink/?linkid=2083731)에 할당 됩니다.
- 삭제할 메시지를 찾을 [콘텐츠 검색을 만듭니다](https://docs.microsoft.com/microsoft-365/compliance/content-search) .
- [보안 및 준수 센터 PowerShell에 연결](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)합니다.

다단계 인증을 사용 하는 경우 [multi-factor authentication을 사용 하 여 Microsoft 365 보안 및 준수 센터 PowerShell에 연결](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)을 참조 하세요.