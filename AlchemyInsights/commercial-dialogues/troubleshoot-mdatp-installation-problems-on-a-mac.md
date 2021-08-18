---
title: Mac에서 MDATP 설치 문제 해결
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4139f47f40a89069521aaa1a3e4fdab56e9e27a2096ae0ad099be827f60d51fc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091046"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Mac에서 MDATP 설치 문제 해결

수동 설치가 실패하면 설치 마법사의 **요약** 페이지에 다음 오류가 표시됩니다.

"설치하는 동안 오류가 발생했습니다. 설치 관리자에서 오류가 발생하여 설치가 실패했습니다. 소프트웨어 제조업체에 문의하여 도움을 요청하세요."

MDM 배포의 경우 페이지에 일반 설치 실패도 표시됩니다.

최종 사용자에게 정확한 오류가 표시되지는는 않습니다. 설치 진행률이 있는 로그 파일은 **/Library/Logs/Microsoft/mdatp/install.log** 에 보관합니다. 각 설치 세션은 이 로그 파일에 추가됩니다. 마지막 설치 세션만 출력하기 위해 를 사용 `sed` 합니다.

자세한 내용은 [Mac용 Microsoft Defender ATP 설치 문제 해결을 참조합니다.](https://go.microsoft.com/fwlink/?linkid=2144615)
