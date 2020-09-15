---
title: Office 앱 업데이트 적용
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
- "1747"
- "9000140"
ms.openlocfilehash: 8306d1acafe48f8779a8c02db8e3fe2f5d5f0e95
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716755"
---
# <a name="apply-updates-for-office-apps"></a>Office 앱 업데이트 적용

기본적으로 Office 앱 업데이트는 무료이고 자동으로 다운로드 되어 관리자가 개입없이 자동으로 백그라운드에서 적용됩니다. 업데이트 적용에 문제가 있어 업데이트를 수동으로 실행하는 경우에는 [Office 업데이트 설치](https://support.office.com/article/install-office-updates-2ab296f3-7f03-43a2-8e50-46de917611c5)를 참조하세요. 자세한 내용은 [Office 설치 문제 해결](https://support.microsoft.com/office/troubleshoot-installing-office-35ff2def-e0b2-4dac-9784-4cf212c1f6c2?ui=en-us&rs=en-us&ad=us#O365Plans=signinorgid)을 참조하세요.

사용자 Office 업데이트를 관리 하려면 다음 옵션을 고려 합니다.

- 원하는 업데이트 빈도에 따라 조직에 알맞는 Office 업데이트 채널을 선택합니다. 방법은 [Microsoft 365 앱의 업데이트 채널 개요](https://docs.microsoft.com/deployoffice/overview-of-update-channels-for-office-365-proplus)를 참조하세요.

- 인터넷 또는 온-프레미스 공유에서 자동으로 업데이트를 적용할지 여부를 결정 합니다. 방법은 [Microsoft 365 앱에 대한 업데이트 관리 방법 선택](https://docs.microsoft.com/deployoffice/choose-how-to-manage-updates-to-office-365-proplus)을 참조하세요.

- Office 업데이트 설정을 검토하여 최종 사용자 컴퓨터에 업데이트를 적용 하는 방법을 제어합니다.

    - [Office 365 앱의 업데이트 설정 구성](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus).
    - [설치 후 Office를 업데이트하는 방법을 정의합니다](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element).

Office 앱을 여러 사용자에게 배포하는 경우 Office 사용자 지정 도구를 사용 하여 배포용 구성 파일을 빌드하고 Office 배포 도구를 사용하여 Office 업데이트를 구성합니다. 자세한 정보는 [Office 사용자 지정 도구 개요](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run) 및 [Office 배포 도구](https://go.microsoft.com/fwlink/p/?LinkID=626065)를 참조하세요.

- Office 업데이트를 배포하는 사용자 그룹을 설정하는 방법에 대한 예시는, [로컬 원본에서 Microsoft 365 앱 배포](https://docs.microsoft.com/deployoffice/deploy-office-365-proplus-from-a-local-source)를 참조하세요.
-   열려 있는 Office 앱 때문에 일부 사용자에게 Office 업데이트가 적용되지 않으면 ForceAppShutdown 설정을 사용하는 것이 좋습니다. 자세한 내용은 [FORCEAPPSHUTDOWN 속성(Property 요소의 일부)](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#forceappshutdown-property-part-of-property-element)를 참조하세요. 

**참고 항목**

[Microsoft 365 앱 업데이트 프로세스 개요](https://docs.microsoft.com/deployoffice/overview-of-the-update-process-for-office-365-proplus).  
[Microsoft 365 앱의 업데이트 릴리스 정보](https://docs.microsoft.com/officeupdates/release-notes-office365-proplus)  
[Microsoft Endpoint Configuration Manager를 사용하여 Microsoft 365 앱의 업데이트 관리](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager)  
