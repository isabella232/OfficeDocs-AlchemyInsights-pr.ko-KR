---
title: 장치에서 iOS 장치를 등록하는 데 Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 0aaece95effa468af5c906a8bd07e5b00ffa3df37b4e2cb296d64108efec94e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54047982"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>장치에서 iOS 장치를 등록하는 데 Microsoft Intune

아래 나열된 리소스를 검토하여 지금 문제를 해결합니다. 
  
몇 가지 일반적인 오류 메시지 및 해결 단계:
  
- **장치 한도 도달** 사용자가 장치 제한보다 더 많은 장치를 등록했습니다. 이러한 문서를 검토하여 장치를 [제거하거나](https://docs.microsoft.com/intune/devices-wipe) 장치 [제한을 변경합니다.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **이 서비스는 지원되지 않습니다. 등록 정책 없음:** APNS(Apple 푸시 알림 서비스)를 구성하거나 갱신해야 합니다. 이 [문서에서 해당](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) 작업을 하는 방법에 대한 지침을 검토하세요. 
    
- **사용자 라이선스 유형이 잘못되었거나 사용자 이름이 인식되지 않습니다.** 사용자에게 Intune 또는 EMS 라이선스를 할당해야 합니다. 다음 문서를 검토하여 관리 센터 [](https://docs.microsoft.com/intune/licenses-assign) 또는 Azure Office [라이선스를 할당합니다.](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
문제를 해결하는 데 도움이 되는 추가 리소스:
  
1. [Intune 문제 해결 포털을](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) 사용하여 일반적인 등록 실패를 진단하고 해결합니다. 자세한 [내용은 이](https://docs.microsoft.com/intune/help-desk-operators) 문서를 검토합니다. 
    
2. 다음 문서를 검토하여 등록과 해결 방법을 방지하는 일반적인 오류의 목록을 확인합니다. [문제 해결 가이드](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) 및 [문제 해결 문서](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).
    
3. [에서 iOS 장치를 등록하는 방법을 Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)
    

