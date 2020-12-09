---
title: Microsoft Edge에 자동으로 로그인
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
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599499"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Microsoft Edge에 자동으로 로그인

Microsoft Edge는 OS의 기본 계정을 사용하여 사용자의 장치가 구성된 방식에 따라 자동으로 사용자에 로그인합니다. 

각 장치 구성 유형 및 해당 종속 사용자 로그인 프로세스의 시나리오는 아래에서 설명합니다.

1. **디바이스가 하이브리드/AAD-J:** 이 옵션은 Windows 10, 다운 수준 Windows 및 해당 서버 버전에서 사용할 수 있습니다. 사용자는 Azure AD(Active Directory) 계정으로 자동으로 로그인됩니다.
2. **디바이스가 도메인에** 가입된 경우: 이 옵션은 Windows 10, 다운 수준 Windows 및 해당 서버 버전에서 사용할 수 있습니다. 기본적으로 도메인 계정이 있는 사용자는 자동으로 로그인되지 않습니다. 자동 로그인을 사용하도록 설정하려면 **ConfigureOnPremisesAccountAutoSignIn 정책을** 사용 합니다. Azure AD 계정이 있는 사용자에 대해 자동 로그인을 사용하도록 설정하려면 디바이스를 하이브리드에 가입하는 것을 고려하세요.
3. **OS의** 기본 계정은 Microsoft 계정입니다. 이 옵션은 Windows 10 RS3(버전 1709, 빌드 10.0.16299) 이상 버전에서 사용할 수 있습니다. 이 시나리오는 엔터프라이즈 장치에서는 발생하지 않습니다. 그러나 OS의 기본 계정이 Microsoft 계정인 경우 Microsoft Edge는 Microsoft 계정을 통해 사용자를 자동으로 로그인합니다.
 
 
