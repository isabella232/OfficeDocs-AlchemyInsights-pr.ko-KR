---
title: RDS엔터프라이즈용 Microsoft 365 앱 터미널 서버 또는 VDI에서 공유하기 위해 배포
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
ms.openlocfilehash: b8df97c19937a757c1de9865b6c7b8d1cddfd62d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325609"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>RDS엔터프라이즈용 Microsoft 365 앱 터미널 서버 또는 VDI에서 공유하기 위해 배포

이전의 엔터프라이즈용 Microsoft 365 앱(RDS)를 사용하여 원격 데스크톱 서비스를 배포하는 경우:

- E Enterprise 3 또는 Microsoft 365 E5와 같이 비즈니스용 Microsoft 365 또는 Office 365 Office 365 Enterprise 요금제가 엔터프라이즈용 Microsoft 365 앱 엔터프라이즈용 Microsoft 365 앱 있어야 합니다.
   **참고:** 비즈니스용 Microsoft 365 앱 Microsoft 365 Business Standard 요금제에 포함된 엔터프라이즈용 Microsoft 365 앱.
- 공유 컴퓨터 [활성화를 사용하도록 설정해야 합니다.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

**참고:** Microsoft 365를 다운로드하고 실행하여 공유 컴퓨터 [지원 및 복구 도우미](https://aka.ms/SaRA_OfficeSCA_M365Portal) 엔터프라이즈용 Microsoft 365 앱 설치할 수 있습니다.

Office 배포 도구를 사용하여 사용자 지정된 설치에 대한 선행 작업, 설정 지침 및 지침에 대한 자세한 내용은 [Deploy 엔터프라이즈용 Microsoft 365 앱 by using Remote Desktop Services를 참조하십시오.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)

공유 컴퓨터 활성화와 관련된 오류를 해결하려면

- 에 대한 공유 컴퓨터 활성화 문제 [엔터프라이즈용 Microsoft 365 앱.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
- [엔터프라이즈용 Microsoft 365 앱 정품 인증 다시 설정](https://go.microsoft.com/fwlink/?linkid=2109218)을 참조하세요.

기본 설치 엔터프라이즈용 Microsoft 365 앱 사용하는 Microsoft 365 관리 센터 RDS에 설치하려면 다음 단계를 사용합니다.

1. 현재 구독을 확인 합니다. [방법을 알아보세요](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. 필요한 경우 다른 구독으로 전환합니다. [방법을 알아보세요](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. 다른 Office RDS 서버에 이미 설치되어 있는 경우 제거합니다. 예를 들어 제어판에서 프로그램   >  **제거로 를 실행합니다.** 문제가 있는 경우 [Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) 지원 및 복구 도우미 사용하여 제거합니다.
4. RDS 서버에서 관리자 계정으로 Microsoft 365 관리 센터 로그인하고 [엔터프라이즈용 Microsoft 365 앱.](https://portal.office.com/OLS/MySoftware.aspx)
5. 설치 Office 후 모든  응용 프로그램을 열거나 로그인하지 Office 않습니다.
6. RDS 서버에서 다음 단계에 따라 레지스트리를 편집하여 공유 컴퓨터 활성화를 사용하도록 설정하십시오.
   1. 화면의 왼쪽 Windows 단추를 마우스 오른쪽 단추로 클릭하고 실행을 **선택합니다.** 열기 상자에 **regedit** 를 입력한 다음 **확인** 을 선택합니다.
   2. 레지스트리 **편집기에서** 장치를 변경할 수 있도록 허용하라는 메시지가 표시될 때 예를 선택합니다.
   3. 레지스트리 편집기에서 \HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\Configuration에서 1로 설정한 **SharedComputerLicensing** 문자열 값을 추가합니다.
   4. RDS 서버에서 최종  사용자로 로그인하고 에서 공유 컴퓨터 활성화가 사용하도록 [설정되어 있는지 엔터프라이즈용 Microsoft 365 앱.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)
