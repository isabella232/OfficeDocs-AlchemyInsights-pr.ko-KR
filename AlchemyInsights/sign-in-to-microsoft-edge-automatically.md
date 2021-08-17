---
title: 자동으로 Microsoft Edge 로그인
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 4e069a1c75caabf3bef7387140edd5650cf966856b888b5c6b5618a603986d6d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050700"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>자동으로 Microsoft Edge 로그인

Microsoft Edge OS 기본 계정을 사용하여 사용자의 장치가 구성된 방식에 따라 자동으로 사용자에 로그인합니다. 

각 유형의 장치 구성 및 해당 종속 사용자 로그인 프로세스의 시나리오는 다음과 같습니다.

- **디바이스가 하이브리드/AAD-J:** 이 옵션은 Windows 10, Windows 버전에서 사용할 수 있습니다. 사용자는 AD(사용자 계정)Azure Active Directory 자동으로 로그인됩니다.
- **장치가 도메인에** 가입된 경우: 이 옵션은 Windows 10, Windows 버전에서 사용할 수 있습니다. 기본적으로 도메인 계정이 있는 사용자는 자동으로 로그인되지 않습니다. 자동 로그인을 사용하도록 설정하려면 **ConfigureOnPremisesAccountAutoSignIn 정책을** 사용 합니다. Azure AD 계정이 있는 사용자에 대해 자동 로그인을 사용하도록 설정하려면 디바이스를 하이브리드에 가입하는 것을 고려하세요.
- **OS의** 기본 계정은 Microsoft 계정입니다. 이 옵션은 Windows 10 RS3(버전 1709, 빌드 10.0.16299) 이상 버전에서 사용할 수 있습니다. 이 시나리오는 엔터프라이즈 장치에서는 발생하지 않습니다. 그러나 OS 기본 계정이 Microsoft 계정인 Microsoft Edge Microsoft 계정으로 사용자를 자동으로 로그인합니다.
 
 
