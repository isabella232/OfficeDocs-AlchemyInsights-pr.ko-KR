---
title: 터미널 서버에 사무실 설치 - 라이선스가 없는 경우
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 35ef317ea87fedd01c08fee5b370e3c81e515c27
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322005"
---
# <a name="installing-office-on-a-terminal-server"></a>터미널 Office 설치

이전 명명된 엔터프라이즈용 Microsoft 365 앱(Windows 데스크톱 서비스)를 사용하여 Windows 서버에 배포하는 경우:
  
- E3 또는 Microsoft 365 E5와 같은 엔터프라이즈용 Microsoft 365 앱 포함된 Office 365 Enterprise 구독이 Enterprise 있습니다. 비즈니스용 Microsoft 365 앱 비즈니스용 Microsoft 365 앱 Premium 계획에는 엔터프라이즈용 Microsoft 365 앱.

- 공유 컴퓨터 [활성화를 사용하도록 설정해야 합니다.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

기본 설치 엔터프라이즈용 Microsoft 365 앱 사용하는 Microsoft 365 관리 센터 RDS에 설치하려면 다음 단계를 사용합니다.

    **Tip**: You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.
  
1. 구독을 Microsoft 365 확인 [방법 알아보기](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. 필요한 경우 다른 구독으로 Microsoft 365 전환합니다. [방법 알아보기](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. 다른 Office 사용하여 RDS 서버에 이미 설치된 Microsoft 365 제거합니다. 예를 들어 제어판으로 가 프로그램을 \> 제거합니다. 문제가 있는 경우 [Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) 지원 및 복구 도우미 사용하여 제거합니다.

4. RDS 서버에서 관리자 계정으로 Microsoft 365 관리 센터 로그인하고 [엔터프라이즈용 Microsoft 365 앱.](https://portal.office.com/OLS/MySoftware.aspx)

5. 설치 Office 후 모든  응용 프로그램을 열거나 로그인하지 Office 않습니다.

6. RDS 서버에서 다음 단계에 따라 레지스트리를 편집하여 공유 컴퓨터 활성화를 사용하도록 설정하십시오.

1. 화면의 왼쪽 Windows 단추를 마우스 오른쪽 단추로 클릭하고 실행을 선택합니다. 열기 상자에 **regedit 를** 입력하고 확인을 선택합니다.

2. 레지스트리 편집기에서 장치를 변경할 수 있도록 허용하라는 메시지가 표시될 때 예를 선택합니다.

3. 레지스트리 편집기에서 \HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\Configuration에서 1로 설정한 **SharedComputerLicensing** 문자열 값을 추가합니다.

7. RDS 서버에서 최종  사용자로 로그인하고 에서 공유 컴퓨터 활성화가 사용하도록 [설정되어 있는지 엔터프라이즈용 Microsoft 365 앱.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)

Office 배포 도구를 사용하여 사용자 지정된 설치에 대한 선행 요구 사항, 설치 지침 및 지침에 대한 자세한 내용은 [Deploy 엔터프라이즈용 Microsoft 365 앱 by using Remote Desktop Services를 참조하십시오.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)
  
공유 컴퓨터 정품 인증과 관련된 오류를 해결하려면 공유 컴퓨터 인증과 관련된 문제 [해결을](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)엔터프라이즈용 Microsoft 365 앱.
  