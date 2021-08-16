---
title: 독립 실행 Teams 또는 새 설치 또는 기존 Office 배포
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: e8baefafc1c2f9583345779c5ae7a9d3d0e05c4b3b7e1b3a74a9a22f7ceed02a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102208"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>독립 실행 Teams 또는 새 설치 또는 기존 Office 배포

Microsoft Teams 새 설치의 일부로  엔터프라이즈용 Microsoft 365 앱, 비즈니스용 Microsoft 365 앱 Mac용 Office. 자세한 내용은 Microsoft Teams 설치에 포함되는 경우를 언제 [Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

또한 현재 채널의 버전 1906부터는 Teams 설치를  최신 버전으로 업데이트할 때 Windows 실행 중인 장치에서 엔터프라이즈용 Microsoft 365 앱(및 비즈니스용 Microsoft 365 앱)의 기존 설치에 Windows 추가됩니다. 자세한 내용은 기존 설치에 대한 정보를 [Office.](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> 이 출시 일정을 기다리지 않는 경우 다음 지침에 따라 사용자에 대해 Teams [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) 독립 실행형으로 배포하거나 사용자가 에서 Teams 설치하도록 할 수 [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) 있습니다.

조직에서 배포할 준비가 Teams 조직의 새 설치 또는 기존 설치에서 Teams 제외하기 [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) 위해 [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) 취할 수 있는 Office.  설치 Teams 있지만 설치한 Teams 자동으로 시작하지 않도록 하려는 경우 설치 후 Microsoft Teams 자동으로 시작하지 못하도록 방지를 [참조합니다.](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)

실행 ***중인 장치에서*** Teams 제거하려면 Windows [제거를 Microsoft Teams.](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81) 여러 대상 Microsoft Teams 사용자로부터 정보를 정리하기 위해 Microsoft Teams [정리를 참조합니다.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

공유 컴퓨터, RDS(원격 데스크톱 서비스) 또는 VDI(가상 데스크톱 인프라)를 사용하는 경우 에서 공유 컴퓨터 및 [VDI 환경을 Microsoft Teams.](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)

If you're using Mac용 Office, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> 설치 Teams 새 기능 및 품질 [](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) 업데이트로 약 2주마다 자동으로 업데이트됩니다. 