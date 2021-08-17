---
title: 감사 로그 검색
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/16/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10964"
- "3100005"
ms.openlocfilehash: 6ca61775d18fb5501911fb3334ef499ff1f06a6b42634367eaf546fc322f822c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57889652"
---
# <a name="retrieve-the-audit-logs"></a>감사 로그 검색

감사 로그를 처음 열면, 해당 로그가 비어 있습니다. 내용을 확인하려면 검색을 수행해야 합니다. 다음은 모든 활동에 대해 일반 검색을 수행하는 방법입니다.

1. 다음 단계 중 하나를 실행합니다.
   - <https://compliance.microsoft.com>의 Microsoft 365 규정 준수 센터에서 **솔루션** \> **감사** 로 이동하세요. 또는 <https://compliance.microsoft.com/auditlogsearch>에서 **감사** 로 직접 이동하세요.
   - <https://security.microsoft.com>의 Microsoft 365 Defender에서 **감사** 로 이동하세요. 또는 <https://sip.security.microsoft.com/auditlogsearch>에서 **감사** 로 직접 이동하세요.

2. **감사** 페이지에서 **검색** 탭이 선택되었는지 확인하고 다음 설정을 구성하세요.
   - **날짜 및 시간 범위**: **시작** 및 **종료** 살자에서 날짜/시간 범위ㄹ르를 선택하세요.
   - **활동**: **모든 활동에 대한 결과 표시** 가 선택되었는지 확인하세요.
   - **사용자**: 모든 사용자에 대한 결과를 반환하려면 빈 기본값을 그대로 사용하거나 한 명 이상의 사용자를 입력합니다.

3. 마쳤으면 **검색** 을 클릭합니다. 활동은 새 **검색 감사** 페이지에 표시됩니다.

4. 결과에서 **결과 필터링** 을 클릭하고 활동 필터링 상자에서 **Set-Mailbox** 를 입력하세요.

5. 결과에서 감사 레코드를 선택합니다. **세부 정보** 플라이아웃에서 **추가 정보** 를 클릭하여 클라이언트, 작업을 수행한 사용자 등과 같은 추가 정보를 확인하세요.
