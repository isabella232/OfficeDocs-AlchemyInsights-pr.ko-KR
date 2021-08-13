---
title: 디바이스에서 Windows 등록하는 문제를 Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a2abb4d0ef5504c496afefe62a80f3fa21c7ec85536e822e402be33b3617b59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981047"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>디바이스에서 Windows 등록하는 문제를 Microsoft Intune

아래 나열된 리소스를 검토하여 지금 문제를 해결합니다.
  
몇 가지 일반적인 오류 메시지 및 해결 단계:
  
 **다음을 위해 소프트웨어를** 설치할 0x80cf4017. 계정 인증서가 만료되었습니다. Intune 관리 콘솔에서 PC 클라이언트 소프트웨어 패키지를 다시 다운로드합니다. 자세한 내용은 이 설명서를 참조하세요.
  
 **오류 코드 0x801c0003:** 이 오류는 다음과 같은 시나리오에서 발생할 수 있습니다.
  
-  사용자가 장치 제한보다 더 많은 장치를 등록했습니다. 이러한 문서를 검토하여 장치를 [제거하거나](https://docs.microsoft.com/intune/devices-wipe) 장치 [제한을 변경합니다.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  "사용자가 장치를 Azure AD에 가입할 수 있습니다."는 "없음"으로 설정됩니다. 전체로 설정하거나 사용자를 선택합니다. 자세한 [내용은 이](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) 설명서를 참조하세요.

-  디바이스가 이미 다른 사용자가 등록했습니다. 이 경우 다시 시도하기 전에 Azure Intune 콘솔에서 장치를 제거하거나 수동으로 디바이스의 구독을 제거합니다.

-  디바이스가 Windows 10 Home. SKUS는 Windows 10 Pro, Education 및 Enterprise SKUS만 Azure Active Directory.

문제를 해결하는 데 도움이 되는 추가 리소스:
  
-  [Intune 문제 해결 포털을](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) 사용하여 일반적인 등록 실패를 진단하고 해결합니다. 자세한 [내용은 이](https://docs.microsoft.com/intune/help-desk-operators) 문서를 검토합니다.

-  다음 문서를 검토하여 등록과 해결 방법을 방지하는 일반적인 오류의 목록을 확인합니다. [문제 해결 가이드](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) 및 [문제 해결 문서](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).

[에서 디바이스를 Windows 등록하는 Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)
