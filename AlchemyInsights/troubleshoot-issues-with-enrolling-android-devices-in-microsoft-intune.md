---
title: Microsoft Intune에서 Android 장치 등록 문제 해결
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830948"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Microsoft Intune에서 Android 장치 등록 문제 해결

아래 나열된 리소스를 검토하여 지금 문제를 해결합니다.
  
몇 가지 일반적인 문제 및 해결 단계:
  
 **회사 포털에서 장치가 암호화되지 않은 오류:** 최신 버전의 Android, 특히 v7.0부터는 디바이스가 완전히 암호화되어 있는지 확인하려면 시작 암호가 필요합니다. 일반적인 솔루션은 시작 핀을 사용하도록 설정하거나 장치를 완전히 암호화하는 것입니다. 자세한 [내용은 이 문서를](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) 검토하세요.
  
 장치가 Intune 서비스로 체크 인하지 못하거나 Intune 관리 콘솔에서 **"Unhealthy"로 표시됩니다.** 일부 Samsung 4.4 및 5.5 장치는 서비스를 체크 인하지 않을 수 있습니다. 이 문제에는 세 가지 가능한 해결 방법도 있습니다.
  
1. Intune 회사 포털 앱을 수동으로 열면 장치 동기화가 자동으로 시작됩니다.

2. 장치를 Android 6.0 이상으로 업데이트합니다.

3. Samsung Smart Manager를 사용하지 않도록 설정하여 Intune 회사 포털을 관리하지 않도록 합니다. 이러한 [문제](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) 및 해결에 대한 자세한 내용은 이 문서를 검토합니다.

 **사용자 라이선스 유형이 잘못되었거나** 사용자 이름을 인식할 수 없습니다 **오류:** 사용자에게 Intune 또는 EMS 라이선스를 할당해야 합니다. 다음 문서를 검토하여 Office Admin Center 또는 Azure Portal을 통해 라이선스를 할당합니다.
  
문제를 해결하는 데 도움이 되는 추가 리소스:
  
1. [Intune 문제 해결 포털을](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) 사용하여 일반적인 등록 실패를 진단하고 해결합니다. 자세한 [내용은 이](https://docs.microsoft.com/intune/help-desk-operators) 문서를 검토합니다.

2. 이 [문서에서](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) 각 오류에 대한 등록 및 해결을 방지하는 일반적인 오류 목록을 검토합니다.

3. [Microsoft Intune에서 Android 장치를 등록하는 방법을 자세히 알아보습니다.](https://docs.microsoft.com/intune/android-enroll)
