---
title: 전자 메일 메시지 회수 또는 바꾸기
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 45882b49c5c47b3e0e4519e2339e6c68110bc75aebeaeac2d0ccd009bdfa3f7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024392"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>전자 메일 메시지의 회수 또는 Microsoft 365

- 조직의 사용자 에게 전송된 메시지만 **회수할 수 있습니다.** 예를 들어 메시지가 Gmail 주소로 전송된 경우 메시지를 회수할 수 없습니다.
- PC에 대해 Outlook **메시지만 회수할 수 있습니다.** 사용자가 Mac용 Outlook 또는 웹용 Outlook 사용하여 메시지를 보내는 경우 다시 호출할 수 없습니다.
- 테넌트 관리자는 **PowerShell을** 사용하여 사용자를 대신하여 메시지를 회수할 수 있습니다(자세한 내용은 다음을 참조하세요. 전자 메일 메시지 검색 및 [삭제).](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)
- 관리 센터에서 보낸 메시지는 회수할 수 없습니다. 자세한 내용은 아래로 스크롤하여 "조직에서 전자 메일 메시지 검색 및 삭제"로 스크롤합니다.

**보낸 전자 메일 메시지 회수 또는 바꾸기**

1. In the folder pane on the left of the Outlook window, choose the Sent Items folder.
2. 회수하려는 메시지를 열 수 있습니다. 메시지를 열려면 두 번 클릭해야 합니다. 읽기 창에 표시하도록 메시지를 선택하면 메시지를 회수할 수 없습니다.
3. 메시지 탭에서 **작업** 회수  >  **이 메시지 를 선택합니다.**
4. 이 **메시지의 언더** 복사본 삭제 또는 **Unread 복사본** 삭제를 선택하고 새 메시지로 바꾸기 를 선택한 다음 확인 을 **선택합니다.**
5. 대체 메시지를 보내는 경우 메시지를 작성한 다음 보내기 를 **선택합니다.**
6. 메시지 회수의 성공 또는 실패는 메시지 회수의 받는 사람 설정에 따라 Outlook.

회수를 검사하는 방법을 비롯한 자세한 내용은 보낸 전자 메일 메시지 회수 또는 [바꾸기를 참조하세요.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

***조직에서 전자*** 메일 메시지를 검색하고 삭제하려면 전역 관리자인 경우 가장 간편합니다. 전역 관리자가 아닌 경우 계정을 eDiscovery 관리자 역할 그룹 또는 준수 검색 관리 역할에 추가해야 합니다. 메시지를 삭제하려면 조직 관리 역할 그룹 또는 검색 및 제거 관리 역할에 가입해야 합니다. 이러한 역할에 대한 사용 권한은 보안 및 준수 & [할당됩니다.](https://protection.office.com/)

1. [삭제할 메시지를 찾는](https://docs.microsoft.com/microsoft-365/compliance/content-search) 콘텐츠 검색을 생성합니다.
2. [보안 및 준수 센터 PowerShell에 연결하기](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)

MFA(다단계 인증)를 사용하는 경우 다단계 인증을 커넥트 보안 Microsoft 365 준수 & [PowerShell을 참조합니다.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
