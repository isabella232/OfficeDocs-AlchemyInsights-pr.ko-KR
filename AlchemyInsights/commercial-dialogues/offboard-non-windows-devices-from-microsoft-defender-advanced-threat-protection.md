---
title: Microsoft Defender ATP(Advanced Threat Protection)에서 비 Windows 장치 오프보딩
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
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736540"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a>Microsoft Defender ATP(Advanced Threat Protection)에서 비 Windows 장치 오프보딩

방법은 다음과 같습니다.

1. 타사 설명서에 따라 Microsoft Defender ATP에서 타사 솔루션 연결을 끊습니다.
2. Azure Active Directory 테넌트에서 타사 솔루션에 대한 사용 권한을 제거합니다.

    1. [Azure 포털](https://go.microsoft.com/fwlink/?linkid=2125612)에 로그인합니다.
    1. 모든 **서비스**  >  **Azure Active Directory** 엔터프라이즈 응용 프로그램을  >  **선택합니다.**
    1. 오프보드할 응용 프로그램을 선택합니다.
    1. **삭제** 를 선택합니다.

자세한 내용은 비 Windows 장치 [오프보드를 참조합니다.](https://go.microsoft.com/fwlink/?linkid=2143630)
