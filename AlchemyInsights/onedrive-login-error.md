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
ms.openlocfilehash: 80aafa2aee7213e1b77d274509a7eb9741c20b525ed97f473093ac8c6514f3c7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54112918"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive 로그인 오류 AADSTS50011

OneDrive 앱에 로그인할 때 "AADSTS50011: 요청에 지정된 회신 URL이 회신과 일치하지 않습니다."라는 오류가 표시될 경우 다음을 확인합니다.

OneDrive 버전이 버전 20.052.XXXX.XXXX보다 크거나 같아야 합니다. 버전을 확인하려면 알림 영역의 파란색 OneDrive 아이콘을 클릭하고 도움말 & 설정 > 설정 > **선택합니다.**

네트워크에서 에 대한 트래픽을 g.live.com **oneclient.sfx.ms.** 해당 트래픽이 차단된 경우 OneDrive 업데이트할 수 없습니다. 네트워크 관리자와 함께 해당 URL에 액세스할 수 있도록 합니다. [이러한 끝점은](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) Microsoft 365 수 있습니다.

현재 버전의 업데이트를 수동으로 다운로드해야 하는 OneDrive [https://aka.ms/getonedrive](https://aka.ms/getonedrive) 방문하세요.
