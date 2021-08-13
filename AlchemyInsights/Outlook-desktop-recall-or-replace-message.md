---
title: Outlook 데스크톱 회수 또는 전자 메일 메시지 바꾸기
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
ms.openlocfilehash: 33fe7ebd53d7ff11dbab54ce589aaf58e68c633be4d83a3cdfb00edc7752430e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918401"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>전자 메일 메시지 Outlook 회수 또는 바꾸기

- 관리자는 **PowerShell을** 사용하여 사용자를 대신하여 메시지를 회수할 수 있습니다. 관리 센터에서 보낸 메시지는 회수할 수 없습니다.
- 조직의 사용자 에게 전송된 메시지만 **회수할 수 있습니다.** 예를 들어 메시지가 Gmail 주소로 전송된 경우 메시지를 회수할 수 없습니다.
- PC에서 보낸 메시지만 Outlook 2016 **수 있습니다.** 사용자가 Mac용 Outlook 또는 웹용 Outlook 사용하여 메시지를 보내는 경우 다시 호출할 수 없습니다.

전자 메일 메시지를 회수하거나 바꾸기 위해

1. 창 왼쪽의 폴더 창에서 Outlook 폴더를 선택합니다.
1. 회수하려는 메시지를 두 번 클릭하여 열 수 있습니다.
1. 메시지 **탭을** 선택한 다음 **작업** 회수  >  **이 메시지 를 선택합니다.**
1. 이 **메시지의 언더** 복사본 삭제 또는 **읽을** 수 없는 복사본 삭제를 선택하고 새 메시지로 바꾸기 를 선택한 다음 확인 을 **선택합니다.**
1. 대체 메시지를 보내는 경우 메시지를 작성한 다음 보내기 를 **선택합니다.**
1. 메시지 회수의 성공 또는 실패는 메시지 회수에 대한 받는 사람의 설정에 Outlook. 회수를 확인할 단계는 이 문서를 [참조하세요.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

조직의 전자 메일 메시지 검색 및 삭제하기

- 전역 관리자가 아닌 경우 메시지를 검색하려면 계정을 eDiscovery 관리자 역할 또는 준수 검색 관리 역할에 추가해야 합니다. 메시지를 삭제하려면 조직 관리 역할 그룹 또는 검색 및 제거 관리 역할에 가입해야 합니다. 이러한 역할에 대한 사용 권한은 보안 및 준수 [센터에서 할당됩니다.](https://go.microsoft.com/fwlink/?linkid=2083731)
- [삭제할 메시지를 찾는](https://docs.microsoft.com/microsoft-365/compliance/content-search) 콘텐츠 검색을 생성합니다.
- [커넥트 및 준수 센터 PowerShell에 대한 정보를 제공합니다.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)

다단계 인증을 사용하는 경우 다단계 인증을 커넥트 Microsoft 365 및 준수 센터 [PowerShell을 참조합니다.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)