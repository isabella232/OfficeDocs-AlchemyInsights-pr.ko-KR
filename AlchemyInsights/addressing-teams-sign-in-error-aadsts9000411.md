---
title: Teams 로그인 오류 AADSTS9000411 해결하기
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 883bf48d3628702c92361a5250f0d59e1352918349b8bc6c3eae5a948b72fc57
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53953037"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Teams 로그인 오류 AADSTS9000411 해결하기

Microsoft Teams에 로그인할 때 다음과 같은 오류가 나타날 수 있습니다. **죄송합니다. 로그인하는 데 문제가 있습니다. AADSTS9000411: 요청의 서식이 잘못 지정되었습니다. "login_hint" 매개 변수가 중복되었습니다.**

이 문제를 해결하려면 Microsoft Teams 클라이언트가 업데이트되어 있는지 확인하세요. 클라이언트 업데이트에 대한 자세한 내용은 [Microsoft Teams 업데이트하기](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)를 참조하세요.

어떤 이유로 클라이언트를 업데이트할 수 없는 경우에는 클라이언트에서 로그오프하면 캐시된 데이터가 대부분 지워집니다. 그러나 로그오프/로그온 후에도 문제가 계속 발생하면 Teams를 종료하고 다음을 수행하여 클라이언트 캐시를 지우세요.
1. Microsoft Teams를 닫습니다.
2. %appdata%\microsoft\teams로 이동하여 모든 파일을 삭제합니다.
3. Microsoft Teams를 다시 엽니다.
