---
title: 사용자 수신 오류, AADSTS7000112 Yammer를 사용할 수 없습니다.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45157337"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>사용자 수신 오류, AADSTS7000112 Yammer를 사용할 수 없습니다.

"AADSTS7000112: 응용 프로그램 '00000005-0000-0ff1-ce00-000000000000'(Yammer)을 사용할 수 없습니다" 라는 오류가 표시되는 경우 Azure AD의 서비스 사용자에게 문제가 있습니다. 관리자가 Yammer에 대한 액세스를 차단하기 위해 서비스 사용자를 비활성화했을 수 있습니다.

서비스 사용자를 비활성화하는 것은 권장되지 않습니다. 추가 문제가 발생할 수 있습니다. Yammer에 대한 사용자 액세스 차단의 지원 방법에 대한 자세한 내용은 [Microsoft 365 사용자에 대한 Yammer 액세스 설정 해제](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access)를 참조하세요.  

Azure 포털에서 이 문제를 해결하고 Yammer에 대한 사용자 액세스를 복원하려면 다음을 수행하세요.

1.  Azure Active Directory 페이지를 열고 왼쪽 탐색 창에서 **관리** 아래에 **Enterprise 응용 프로그램**을 선택합니다.
3.  검색 상자에 **Office 365 Yammer**를 입력하고 응용 프로그램 이름을 선택하여 설정을 엽니다.
4.  왼쪽 탐색 창의 **관리**에서 **속성**을 선택합니다.
5.  **사용자가 로그인할 수 있도록 설정하시겠습니까?** 의 값을 **예**로 설정하고 **저장**을 선택합니다.
6.  Yammer에 다시 로그인합니다. 쿠키를 삭제해야 할 수 있습니다.

또는 PowerShell 명령을 실행하여 값을 설정할 수 있습니다. 자세한 내용은 [Office 365에서 Yammer 타일을 클릭할 때 "죄송합니다. 로그인 문제가 발생했습니다" 오류](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365)를 참조하세요. 