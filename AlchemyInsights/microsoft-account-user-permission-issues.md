---
title: 문제 해결 - 디렉터리에 사용자를 찾을 수 없습니다.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 79429f8e9523ad6b08cd2cd2b19dd221bac797d00de142cbb18826b86fb5ae4e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098176"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>문제 해결 - 디렉터리에 사용자를 찾을 수 없습니다.

디렉터리에서 "사용자를 찾을 수 없습니다."라는 오류 메시지가 표시될 경우 문제 유형이 디렉터리에 없는 경우 다시 시도하세요.

다음 단계를 완료하여 문제를 해결할 수 있습니다.

- 전자 메일 초대를 수락한 계정이 나중에 로그인하는 데 사용되는 계정과 동일한지 확인 사용자가 동일한 계정을 사용하여 초대를 수락하고 사이트에 로그인하는지 확인 

자세한 내용은 Microsoft 계정의 별칭을 관리하여 앱 로그인을 [ </a> 관리하는 Microsoft 365 참조하세요.](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases) 

- 사용자가 오류를 수신하는 각 사이트로 검색합니다. 

사이트 URL의 끝에 "/_layouts/15/people.aspx/membershipgroupid=0"(이중 따옴표 안에)을 추가합니다. 

예: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- 목록에서 사용자를 선택합니다.

- **리본에서 사용자 권한** 제거를 클릭합니다. 
-  사용자를 다시 추가하고 사용자에게 초대를 다시합니다.

