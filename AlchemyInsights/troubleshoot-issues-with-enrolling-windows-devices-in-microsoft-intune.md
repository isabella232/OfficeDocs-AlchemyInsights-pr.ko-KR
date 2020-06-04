---
title: Microsoft Intune에서 Windows 장치 등록 문제 해결
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665838"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Microsoft Intune에서 Windows 장치 등록 문제 해결

아래에 나열 된 리소스를 검토 하 여 지금 문제를 해결 하세요.
  
몇 가지 일반적인 오류 메시지 및 해결 단계:
  
 **소프트웨어를 설치할 수 없음, 0x80cf4017:** 계정 인증서가 만료 되었습니다. Intune 관리 콘솔에서 PC 클라이언트 소프트웨어 패키지를 다시 다운로드 합니다. 자세한 내용은이 설명서를 참조 하십시오.
  
 **오류 코드 0x801c0003:** 이 오류는 다음과 같은 경우에 발생할 수 있습니다.
  
-  사용자에 게 장치 제한 보다 많은 디바이스가 등록 되어 있습니다. 이러한 문서를 검토 하 여 [장치를 제거](https://docs.microsoft.com/intune/devices-wipe) 하거나 [장치 제한을 변경](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)합니다.

-  "사용자가 Azure AD에 장치를 연결할 수 있습니다."가 "없음"으로 설정 됩니다. 모두로 설정 하거나 사용자를 선택 합니다. 자세한 내용은 [이 설명서](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) 를 참조 하십시오.

-  다른 사용자가 장치를 이미 등록 했습니다. 이 경우에는 다시 시도 하기 전에 Azure Intune 콘솔에서 장치를 제거 하거나 장치를 수동으로 등록 취소 해야 합니다.

-  장치가 Windows 10 Home입니다. Windows 10 Pro, 교육 및 Enterprise Sku만 Azure Active Directory에 참가할 수 있습니다.

문제를 해결 하는 데 도움이 되는 추가 리소스:
  
-  [Intune 문제 해결 포털](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) 을 사용 하 여 일반적인 등록 오류를 진단 하 고 해결 합니다. 자세한 내용을 보려면 [이 문서](https://docs.microsoft.com/intune/help-desk-operators) 를 검토 하세요.

-  다음 문서를 검토하여 등록과 해결 방법을 방지하는 일반적인 오류의 목록을 확인합니다. [문제 해결 가이드](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) 및 [문제 해결 문서](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Microsoft Intune에서 Windows 장치를 등록 하는 방법에 대해 알아봅니다](https://docs.microsoft.com/intune/windows-enroll).
