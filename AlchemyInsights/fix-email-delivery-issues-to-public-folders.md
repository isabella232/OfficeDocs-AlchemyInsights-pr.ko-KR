---
title: 메일 사용 가능 공용 폴더에 대한 전자 메일 배달 문제 해결
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
- "1956"
- "3500007"
ms.openlocfilehash: ff1400f694ae037a8658356af068b4c20b8fa9d9908dafedb90db7bb6859530f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068818"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>메일 사용 가능 공용 폴더에 대한 전자 메일 배달 문제 해결

외부 보낸 사람이 메일 사용 가능 공용 폴더로 메시지를 보낼 수 없는 경우 보낸 사람이 다음 오류를 수신하는 경우: 찾을 수 **없습니다(550 5.4.1)** 공용 폴더의 전자 메일 도메인이 내부 릴레이 도메인 도메인으로 구성되어 있는지 확인합니다.

1. [EAC(Exchange 관리 센터)를 열 수 있습니다.](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. 메일 흐름 **허용** \> **도메인으로** 이동하여 허용 도메인을 선택한 다음 편집을 **클릭합니다.**

3. 도메인 유형이 **Authoritative로** 설정된 경우 열릴 속성 페이지에서 값을  내부 릴레이로 변경한 다음 저장을 **클릭합니다.**

외부 보낸 사람이 사용 권한이 없는 **경우(550 5.7.13)** 오류가 발생하면 Exchange Online [PowerShell에서](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) 다음 명령을 실행하여 공용 폴더의 익명 사용자에 대한 사용 권한을 확인합니다.

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` 예를 들면 `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` 입니다.

외부 사용자가 이 공용 폴더로 전자 메일을 보낼 수 있도록 허용하기 위해 사용자 익명에 CreateItems 액세스 권한을 추가합니다. 예를 들면 `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`와 같습니다.
