---
title: 장치 사용
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
- "9003257"
- "8278"
ms.openlocfilehash: 4722ccf6847fc6c02616dbc62d59a2a87c089f77ae79c0a916211af6c5f2a6d0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003492"
---
# <a name="enable-device"></a>장치 사용

**Powershell 명령을 사용하여 디바이스를 사용하도록 설정하려면**

다음의 명령을 실행합니다.

- 장치 개체를 얻은 경우: `Get-MsolDevice -Name <Name>`
- 디바이스를 사용하도록 설정하려면: `Enable-MsolDevice -DeviceId <DeviceId>`

관리되는 도메인에서 하이브리드 가입 구성에 대한 자세한 내용은 [Configure Hybrid Join을 참조하십시오.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains)
