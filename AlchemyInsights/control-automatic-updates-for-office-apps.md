---
title: Office 앱에 대한 자동 업데이트 제어
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: ab3d6e60bc1b67220adbdf7ba61599a6b7aa663a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747782"
---
# <a name="control-automatic-updates-for-office-apps"></a>Office 앱에 대한 자동 업데이트 제어

기본적으로 Office 앱에 대한 업데이트는 자동으로 다운로드되어 사용자 개입 없이 백그라운드에서 적용됩니다. 그러나 관리자는 Office 업데이트 설정을 사용하여 업데이트를 적용하는 방법을 제어할 수 있습니다. 업데이트 설정을 사용하면 관리자가 자동 업데이트를 사용하거나 사용하지 않도록 설정하고, Office에서 **지금 업데이트** 단추를 표시하거나 숨기고, 업데이트 마감일을 설정하는 등 다양한 작업을 할 수 있습니다. 자세한 내용은 다음을 참조하세요.

- [Office의 업데이트 설정 구성](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Office의 자동 업데이트를 사용할 수 없음](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [설치 후 Office를 업데이트하는 방법 정의](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

클라이언트 머신에 적용된 기존 업데이트 설정을 검토하려면 다음 단계를 따릅니다.

1. **시작** > **실행** > **regedit**로 이동하여 레지스트리 편집기를 엽니다.
2. 다음 위치로 전환하고 Office 업데이트 설정을 검토합니다.  
    a. HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\  
    b. ClickToRun\Configuration

**참고**  OfficeMgmtCOM 키가 설정되어 있는 경우 **Office** > **계정** > **Office 업데이트**에 "업데이트는 시스템 관리자가 관리합니다."라는 메시지가 표시될 수 있습니다. 자세한 내용은 [Microsoft Endpoint Configuration Manager를 사용하여 Microsoft 365 앱으로의 업데이트 관리하기](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager)를 참조하세요.  