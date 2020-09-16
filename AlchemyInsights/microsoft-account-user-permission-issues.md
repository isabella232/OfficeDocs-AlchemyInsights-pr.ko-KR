---
title: 문제 해결-디렉터리에서 사용자를 찾을 수 없음
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725413"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>문제 해결-디렉터리에서 사용자를 찾을 수 없음

사용자가 디렉터리에서 "사용자를 찾을 수 없습니다." 라는 오류 메시지가 표시 되는 경우 문제 유형이 디렉터리에 없는 사용자 인 경우 다시 시도 하세요.

문제를 해결 하기 위해 다음 단계를 완료할 수 있습니다.

- 전자 메일 초대를 수락한 계정이 나중에 로그인 하는 데 사용 되는 것과 동일한 계정 인지 확인 합니다. 사용자가 초대를 수락 하 고 사이트에 로그인 하는 데 동일한 계정을 사용 하 고 있는지 확인 합니다. 

자세한 내용은 microsoft [계정을 </a> 365 관리 하기 위해 microsoft 계정의 별칭을 관리](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)하는 방법을 참조 하세요. 

- 사용자에 게 오류를 수신 하는 각 사이트로 이동 합니다. 

사이트 URL 끝에 "/_layouts/15/people.aspx/membershipgroupid = 0" (이중 따옴표 내)을 추가 합니다. 

예: https://< "contoso" sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0 >.

- 목록에서 사용자를 선택 합니다.

- 리본에서 **사용자 권한 제거** 를 클릭 합니다. 
-  사용자를 추가 하 고 사용자에 게 초대를 다시 보냅니다.

