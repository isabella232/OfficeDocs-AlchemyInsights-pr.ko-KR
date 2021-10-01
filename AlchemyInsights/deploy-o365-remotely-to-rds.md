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
ms.openlocfilehash: 9d928a3bf58dedc3aaf231c8a051f87b0bbdf438
ms.sourcegitcommit: 391052026a6ce7646926d233d0fd9ba135088f79
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/01/2021
ms.locfileid: "60041012"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>RDS엔터프라이즈용 Microsoft 365 앱 터미널 서버 또는 VDI에서 공유하기 위해 배포

이전의 Microsoft 365 앱(원격 데스크톱 서비스)를 사용하여 배포하려면 다음을 해야 합니다.

- 이전 버전의 Windows(예: Windows 7 SP1, Windows Server 2008 R2)를 실행하는 경우 간단한 수정을 사용하여 TLS 1.2를 기본값으로 사용하도록 설정할 수 있습니다. 쉬운 수정 및 자세한 내용은 업데이트 를 참조하여 의 [WinHTTP에서 TLS 1.1 및 TLS 1.2를](https://support.microsoft.com/en-us/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy)기본 보안 프로토콜로 Windows. 
- 추가(이전에는 엔터프라이즈용 Microsoft 365 앱 Plus)를 포함하는 Office 365 있습니다. 예를 들어 Office 365 E3 Microsoft 365 E5 또는 Project 또는 Visio 데스크톱 버전(예: Project 플랜 3 또는 Visio 플랜 2) 또는 Microsoft 365 Business Premium 계획(비즈니스용 Microsoft 365 앱.
- 공유 컴퓨터 활성화를 사용하도록 설정 자세한 내용은 Overview [of shared computer activation for Microsoft 365 앱.](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation)

**참고:** 공유 컴퓨터 Microsoft 365 앱 모드로 설치하려면 [Microsoft](https://docs.microsoft.com/alchemyinsights/deploy-o365-remotely-to-rds)지원 및 복구 도우미. Office 배포 도구를 사용하여 설치를 사용자 지정하는 선행 요구 사항, 설정 지침 및 지침에 대한 자세한 내용은 [Deploy Microsoft 365 앱 by using Remote Desktop Services를 참조하십시오.](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services)

공유 컴퓨터 활성화와 관련된 오류를 해결하려면 다음을 참조합니다.

- [공유 컴퓨터 인증과 관련한 문제 Microsoft 365 앱](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [엔터프라이즈용 Microsoft 365 앱 정품 인증 상태 초기화](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

기본 설치 Microsoft 365 앱 사용하는 Microsoft 365 관리 센터 RDS에 RDS를 설치하려면 다음 단계를 수행합니다.

1. 계획 Microsoft 365 확인 자세한 내용은 [어떤 구독이 있나요? 을 참조하세요.](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

1. 필요한 경우 다른 요금제로 Microsoft 365 전환합니다. 자세한 내용은 [Upgrade to a different plan을 참조하십시오.](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan)

1. 다른 Microsoft 365 앱 사용하여 RDS 서버에 이미 설치되어 있는 경우 제어판 프로그램 제거로 하여   >  **제거합니다.** 문제가 있는 경우 Microsoft 지원 및 복구 도우미 [다운로드하여 제거합니다.](https://aka.ms/SARA-OfficeUninstall-Alchemy)

1. RDS 서버에서 관리자 계정으로 Microsoft 365 관리 센터 로그인하고 를 [Office.](https://portal.office.com/OLS/MySoftware.aspx)

   설치 Office 후 모든 응용 프로그램을 열거나 로그인하지 Office 않습니다.

1. RDS 서버에서 레지스트리를 편집하여 공유 컴퓨터 활성화를 사용하도록 설정합니다.

   1. 화면의 왼쪽 Windows 단추를 마우스 오른쪽 단추로 클릭하고 실행을 **선택합니다.** 열기 상자에 **regedit** 를 입력한 다음 **확인** 을 선택합니다.

   1. 레지스트리 편집기에서 장치를 변경할 수 있도록 허용하라는 메시지가 표시될 때 예를 **선택합니다.**

   1. 레지스트리 편집기에서 HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration에서 설정 1을 사용하여 **SharedComputerLicensing의** 문자열 값을 **추가합니다.**

1. RDS 서버에서 최종 사용자로 로그인하고 공유 컴퓨터 활성화가 사용자에 대해 사용하도록 설정되어 있는지 Microsoft 365 앱. 

   자세한 내용은 [에 대해 공유 컴퓨터](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps)활성화가 사용하도록 설정되어 있는지 Microsoft 365 앱.