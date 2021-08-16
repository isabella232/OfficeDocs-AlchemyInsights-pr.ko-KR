---
title: Teams 4c7 오류 발생
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: ea3e8f23c07103e604fc6b264047582b9c3e26b6b73237adc30eba574e06cfd3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049314"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7 오류 Microsoft Teams

이 오류는 양식 Microsoft Teams 필요하기 때문에 발생합니다. AD FS(Active Directory Federation Services)를 배포할 때 기본적으로 인트라넷에 대해 폼 인증을 사용할 수 없습니다. 통합 Windows 실패하면 폼 인증을 사용하여 로그인하라는 메시지가 표시될 수 있습니다.

이 문제를 해결하려면 Active Directory의 로컬 복사본이 있는 컴퓨터에서 AD FS MMC(Microsoft Management Console) 스냅인을 사용하여 폼 인증을 사용하도록 설정하십시오. 이렇게 하려면 다음과 같이 하십시오. 

1. 탐색 창에서 인증 **정책으로 이동합니다.**
2. 세부 **정보** 창의 작업에서 전역 기본 인증 **편집을 선택합니다.**
3. **인트라넷 탭에서** 폼 **인증을 선택합니다.**
4. **확인(또는** **적용)을 선택합니다.**