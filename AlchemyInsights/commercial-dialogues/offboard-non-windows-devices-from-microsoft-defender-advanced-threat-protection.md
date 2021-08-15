---
title: Microsoft Defender ATP(Windows Threat Protection)에서 비구성 장치 온보딩
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
ms.openlocfilehash: fbaab348e06691b73db68492a0083c4a5a54c4504e03d27ec53f2a9f5047266d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53967807"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a>Microsoft Defender ATP(Windows Threat Protection)에서 비구성 장치 온보딩

방법은 다음과 같습니다.

1. 타사 설명서에 따라 Microsoft Defender ATP에서 타사 솔루션 연결을 끊습니다.
2. 테넌트 Azure Active Directory 타사 솔루션에 대한 사용 권한을 제거합니다.

    1. [Azure 포털](https://go.microsoft.com/fwlink/?linkid=2125612)에 로그인합니다.
    1. 응용 **프로그램 및**  >  **Azure Active Directory**  >  **Enterprise 선택합니다.**
    1. 오프보드할 응용 프로그램을 선택합니다.
    1. **삭제** 를 선택합니다.

자세한 내용은 비보안 장치 를 Windows [참조합니다.](https://go.microsoft.com/fwlink/?linkid=2143630)
