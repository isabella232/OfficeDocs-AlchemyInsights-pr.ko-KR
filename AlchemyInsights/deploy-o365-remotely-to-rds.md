---
title: RDS, 터미널 서버 또는 VDI에서 공유 사용을 위해 엔터프라이즈용 Microsoft 365 앱 배포
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200679"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>RDS, 터미널 서버 또는 VDI에서 공유 사용을 위해 엔터프라이즈용 Microsoft 365 앱 배포

이전 명명된 터미널 서비스인 원격 데스크톱 서비스(RDS)를 사용하여 엔터프라이즈용 Microsoft 365 앱을 배포하는 경우:

- 비즈니스용 Microsoft 365 요금제 또는 엔터프라이즈용 Microsoft 365 앱을 포함하는 Office 365 요금제(예: Office 365 Enterprise E3 또는 Enterprise E5)가 있어야 합니다.
   > [!NOTE]
   > 비즈니스용 Microsoft 365 앱 및 Microsoft 365 Business Standard 요금제에는 엔터프라이즈용 Microsoft 365 앱이 포함되어 있지 않습니다.
- 공유 컴퓨터 [활성화를 사용하도록 설정해야 합니다.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

> [!NOTE]
> Microsoft 지원 및 복구 [](https://aka.ms/SaRA_OfficeSCA_M365Portal) 도우미를 다운로드하여 실행하여 공유 컴퓨터 활성화 모드로 엔터프라이즈용 Microsoft 365 앱을 설치할 수 있습니다.

Office 배포 도구를 사용하여 사용자 지정된 설치에 대한 선행 작업, 설정 지침 및 지침에 대한 자세한 내용은 [Deploy Microsoft 365 Apps for Enterprise by using Remote Desktop Services를 참조하십시오.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)

공유 컴퓨터 활성화와 관련된 오류를 해결하려면

- 엔터프라이즈용 Microsoft 365 앱에 대한 공유 [컴퓨터 활성화 문제 해결을 참조하세요.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
- [엔터프라이즈용 Microsoft 365 앱 정품인증 재설정](https://go.microsoft.com/fwlink/?linkid=2109218)을 참고하세요.

기본 설치 설정을 사용하는 Microsoft 365 관리 센터에서 RDS에 엔터프라이즈용 Microsoft 365 앱을 설치하려면 다음 단계를 사용합니다.

1. 현재 구독을 확인 합니다. [방법을 알아보세요](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. 필요한 경우 다른 구독으로 전환합니다. [방법을 알아보세요](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. Office가 다른 Microsoft 구독을 사용하여 RDS 서버에 이미 설치되어 있는 경우 제거합니다. 예를 들어 제어판에서 프로그램   >  **제거로 를 실행합니다.** 문제가 있는 [경우 Microsoft 지원](https://aka.ms/SARA-OfficeUninstall-Alchemy) 및 복구 도우미를 사용하여 제거합니다.
4. RDS 서버에서 관리자 계정으로 Microsoft 365 관리 센터에 로그인하고 엔터프라이즈용 [Microsoft 365 앱을 설치합니다.](https://portal.office.com/OLS/MySoftware.aspx)
5. Office를 설치한 후 Office 응용 프로그램을 ***열거나*** 로그인하지 않습니다.
6. RDS 서버에서 다음 단계에 따라 레지스트리를 편집하여 공유 컴퓨터 활성화를 사용하도록 설정하십시오.
   1. 화면의 왼쪽 아래 모서리에 있는 Windows 단추를 마우스 오른쪽 단추로 클릭하고 실행을 **선택합니다.** 열기 상자에 **regedit** 를 입력한 다음 **확인** 을 선택합니다.
   2. 레지스트리 **편집기에서** 장치를 변경할 수 있도록 허용하라는 메시지가 표시될 때 예를 선택합니다.
   3. 레지스트리 편집기에서 \Office\ClickToRun\Configuration에서 1로 설정한 **SharedComputerLicensing의** HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft 추가합니다.
   4. RDS 서버에서 최종  사용자로 로그인하고 엔터프라이즈용 [Microsoft 365 앱에](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)대해 공유 컴퓨터 활성화가 사용하도록 설정되어 있는지 확인합니다.
