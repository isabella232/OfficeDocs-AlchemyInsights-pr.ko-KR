---
title: 메일 사용이 가능한 공용 폴더에 대 한 전자 메일 배달 문제 해결
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 45665f900014c52e6a920325b0a3b0f6f79fb72d
ms.sourcegitcommit: d1c1d5bcb52ba9083e8dd7603feb72436c5154c8
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/17/2019
ms.locfileid: "31910609"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>메일 사용이 가능한 공용 폴더에 대 한 전자 메일 배달 문제 해결

외부 보낸 사람이 메일 사용이 가능한 공용 폴더에 메시지를 보낼 수 없고 보낸 사람에 게 오류를 찾을 수 없는 경우 **(550 5.4.1)**, 공용 폴더에 대 한 전자 메일 도메인이 대신 내부 릴레이 도메인으로 구성 되었는지 확인 합니다. 신뢰할 수 있는 도메인:

1. [EAC (Exchange 관리 센터)](https://docs.microsoft.com/Exchange/exchange-admin-center)를 엽니다.

2. **메일 흐름** \> **허용 도메인**으로 이동 하 여 허용 도메인을 선택한 다음 **편집**을 클릭 합니다.

3. 해당 도메인 유형이 **신뢰할**수 있는 것으로 설정 된 경우 열리는 속성 페이지에서 해당 값을 **내부 릴레이로** 변경 하 고 **저장**을 클릭 합니다.

외부 보낸 사람에 **게 사용 권한이 없는 오류 (550 5.7.13)** 가 수신 되는 경우 [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) 에서 다음 명령을 실행 하 여 공용 폴더의 익명 사용자에 대 한 사용 권한을 확인 합니다.

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`예를 `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`들면입니다.

외부 사용자가이 공용 폴더에 전자 메일을 보낼 수 있도록 하려면 사용자 익명에 createitems 액세스 권한을 추가 합니다. 예를 들면 `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`와 같습니다.