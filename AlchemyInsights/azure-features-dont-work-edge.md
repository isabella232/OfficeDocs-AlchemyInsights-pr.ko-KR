---
title: Azure 기능이 Microsoft Edge에서 제대로 작동하지 않는 경우 수행할 작업
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8315"
- "9004429"
ms.openlocfilehash: aa89cbd58875f418a0a7a9db4b5eb4f0e4c1223a
ms.sourcegitcommit: e9fcd72e64d35f5ba14dfa0fbde39eae20d86cfe
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/27/2021
ms.locfileid: "53603295"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Azure 기능이 Microsoft Edge에서 제대로 작동하지 않는 경우 수행할 작업

Microsoft Edge에는 Azure 사용자가 Windows 관리 센터에 로그인하는 방법에 영향을 줄 수 있는 보안 영역과 관련된 알려진 문제가 있습니다. 자세한 내용은 [Edge의 알려진 문제](https://go.microsoft.com/fwlink/?linkid=2140608)를 참조하세요. Microsoft Edge에서 Azure 기능을 사용하는 데 문제가 있는 경우 다음을 시도해 보세요.

1. 시작 메뉴의 **검색** 표시줄에 **인터넷 옵션** 을 입력한 다음 선택합니다.
1. **인터넷 속성** 에서 **보안** 탭을 선택합니다.
1. **신뢰할 수 있는 사이트** 를 선택한 다음 **사이트** 를 선택합니다.
1. 게이트웨이 URL과 <https://login.microsoftonline.com> 및 <https://login.live.com>을(를) 추가하고 **닫기** 를 선택합니다.
1. **인터넷 속성** 에서 **개인 정보** 탭을 선택합니다.
1. 팝업 차단기 섹션에서 **설정** 을 선택합니다. 게이트웨이 URL과 <https://login.microsoftonline.com> 및 <https://login.live.com>을(를) 추가한 다음 **닫기** 를 선택합니다.