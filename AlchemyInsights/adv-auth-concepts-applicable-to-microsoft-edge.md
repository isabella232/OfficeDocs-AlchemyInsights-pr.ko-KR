---
title: 사용자에 적용할 수 있는 고급 인증 Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: 8ddec37260ec4e3bcc390dcc8adb7397368de19555ee31be458be033d3886386
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934371"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>사용자에 적용할 수 있는 고급 인증 Microsoft Edge

다음은 사용자에 적용할 수 있는 고급 인증 Microsoft Edge.

**사전 인증**

[ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) 정책을 사용하도록 설정하면 Microsoft Edge 인증을 통해 로그인한 사용자를 사전 인증하려고 Microsoft 서비스. 정기적으로 온라인 서비스를 사용하여 사전 인증을 관리하는 구성이 포함된 업데이트된 매니페스트를 검사합니다.

이점: 사전 인증을 사용하면 새 탭 페이지와 같은 Office 인증을 사용할 수 있습니다. 또한 검색 Bing 사용하는 경우 사전 인증을 사용하면 주소 표시줄의 성능이 향상되어 비즈니스 요구에 맞게 개인 설정된 검색 결과를 생성할 수 있습니다.

**Windows Hello NTLM 인증용 CredUI**

웹 사이트에서 NTLM 또는 협상 메커니즘을 통해 사용자에 로그인할 때 SSO(Single Sign-On)를 사용할 수 없는 경우 이 기능을 사용하면 사용자가 자격 증명 Cred UI를 사용하여 웹 사이트와 OS 자격 증명을 공유하고 인증 Windows Hello 수 있습니다. 이 로그인 흐름은 NTLM Windows 10 협상 챌린지 중에 SSO를 얻지 않은 사용자에게만 표시됩니다.

**저장된 암호를 사용하여 자동으로 로그인**

암호를 저장하는 Microsoft Edge 자격 증명을 저장한 웹 사이트에 대한 자동 로그인을 사용하도록 설정할 수 있습니다. 사용자는 이 기능을 설정하거나 해제할 수 edge://settings/passwords 암호 관리자 정책에서 [구성할 수](https://go.microsoft.com/fwlink/?linkid=2134622) 있습니다.
