---
title: OneDrive 로그인 오류 AADSTS50011
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
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947503"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive 로그인 오류 AADSTS50011

OneDrive 앱에 로그인 할 때 "AADSTS50011: 요청에 지정 된 회신 URL이 reply와 일치 하지 않습니다." 라는 오류가 표시 되 면 다음을 확인 합니다.

OneDrive 버전은 20.052 버전 보다 크거나 같아야 합니다. XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX. 버전을 확인 하려면 알림 영역에서 파란색 OneDrive 아이콘을 클릭 하 고 **도움말 & 설정 > 설정 >** 를 선택 합니다.

네트워크가 **g.live.com** 및 **oneclient.sfx.ms** 로의 트래픽을 차단할 수도 있습니다. 해당 트래픽이 차단 되 면 OneDrive에서 자체적으로 업데이트할 수 없습니다. 네트워크 관리자와 협력 하 여 해당 Url에 대 한 액세스 권한이 있는지 확인 합니다. [이러한 끝점](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) 은 Microsoft 365 계획을 사용 하는 고객에 게 연결할 수 있어야 합니다.

최신 버전의 OneDrive를 수동으로 가져오려면 다음을 방문 하세요 [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
