---
title: '오류: 이 컴퓨터의 규칙이 일치하지 않습니다.'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782958"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>오류: 이 컴퓨터의 규칙이 일치하지 않습니다.

이 알려진 문제의 업데이트된 상태를 확인하려면 이 컴퓨터의 규칙이 Microsoft Exchange의 규칙과 [일치하지 않습니다.를 참조합니다.](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

The Outlook Team has implemented a fix in Build 12928.10000. The fix is already at Insider Fast and will go to Monthly Channel in late June 2020. 고정 빌드가 있는 경우 마지막으로 "유지할 규칙"을 묻는 메시지가 표시될 수 있습니다. 메시지가 표시될 때 서버를 선택한 다음 Outlook에서 다시 돌아가 사용하지 않도록 설정한 규칙을 다시 사용하도록 설정하십시오.

수정을 사용할 수 있는 경우 다음 해결 방법을 사용하시기 바랍니다.

**해결 프로그램:** 최근 보고서에서 Outlook 데스크톱에서 클라이언트 규칙만 만든 사용자에 대해 문제가 발생했습니다. 문제가 계속 발생하면 규칙을 삭제한 다음 문제가 해결될 때까지 OWA(Outlook Web App)에서만 규칙을 만들고 편집하는 것이 있습니다.

규칙을 수동으로 삭제할 수 없는 경우 /cleanrules /cleanrules를 실행하여 Outlook을 시작할 때 Outlook 명령을 Outlook.exe 있습니다. 그러면 클라이언트 및 서버 규칙이 모두 삭제됩니다. Outlook 프로필의 모든 계정에 대한 모든 규칙이 삭제됩니다. 이 명령은 명령줄 스위치 문서에 더 설명되어 있습니다.

