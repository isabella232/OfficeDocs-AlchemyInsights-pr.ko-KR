---
title: Microsoft Edge에서 Azure 기능이 제대로 작동하지 않는 경우의 작업
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576483"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Microsoft Edge에서 Azure 기능이 제대로 작동하지 않는 경우의 작업

Microsoft [Edge에는](https://go.microsoft.com/fwlink/?linkid=2140608) 보안 영역과 관련된 알려진 문제가 있으며 Azure 사용자가 Windows Admin Center에 로그인하는 방식에 영향을 줄 수 있습니다. Microsoft Edge에서 Azure 기능을 사용하는 데 문제가 있는 경우 다음 단계를 시도해 하세요.

1. 시작 **메뉴에서** 인터넷 옵션을 **검색하고** 선택합니다.
2. 인터넷 속성 **대화 상자에서** 보안 **탭으로** 이동하십시오.
3. 신뢰할 수 **있는 사이트 영역과** 사이트 **단추를** 선택합니다.
4. 신뢰할 수 **있는 사이트** 대화 상자에서 게이트웨이 URL도 추가하고 [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) 닫기를 **선택합니다.**
5. 인터넷 속성 **대화 상자에서** 개인 정보 **탭으로** 이동하십시오.
6. 팝업 차단 **섹션에서** 설정을 **선택합니다.** 대화 상자가 열리면 게이트웨이 URL도 추가하고 [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) 닫기를 **선택합니다.**
