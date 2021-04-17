---
title: Office 업데이트와 함께 설치된 Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2599"
- "9000140"
- "9000660"
- "2509"
ms.openlocfilehash: 36b0b1a7bf37c27304b4124157dba9aba337678c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51832388"
---
# <a name="microsoft-teams-installed-with-office-updates"></a>Office 업데이트와 함께 설치된 Microsoft Teams

Microsoft Teams는 엔터프라이즈용  Microsoft 365 앱, 비즈니스용 Microsoft 365 앱 및 Mac용 Office의 새 설치의 일부로 포함됩니다. 자세한 내용은 언제 Microsoft Teams가 Office의 새 설치에 포함 [되나요?를 참조하세요.](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

또한 현재 채널의 버전 1906부터는 기존 설치를  최신 버전으로 업데이트할 때 Windows를 실행하는 장치에서 엔터프라이즈용 Microsoft 365 앱(및 비즈니스용 Microsoft 365 앱)의 기존 설치에 Teams가 점진적으로 추가됩니다. 자세한 내용은 Office의 기존 설치에 대한 [정보를 참조하세요.](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

**참고:** 이 출시 일정을 기다리지 않는 경우 다음 지침에 따라 사용자를 위한 독립 [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)실행형으로 Teams를 배포하거나 사용자가 에서 Teams를 직접 설치하도록 할 수 https://teams.microsoft.com/downloads 있습니다.

조직에서 Teams를 배포할 준비가 되어 있지 않은 [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) 경우 [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) Office의 신규 또는 기존 설치에서 ***Teams를*** 제외할 수 있습니다. Teams를 설치하겠지만 Teams가 설치된 후 사용자를 위해 자동으로 시작하지 않도록 하려는 경우 설치 후 Microsoft Teams가 자동으로 시작되지 않도록 방지를 [참조합니다.](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)

Windows를 실행하는 장치에서 ***Teams를*** 제거하려면 [Microsoft Teams 제거를 참조하세요.](https://support.office.com/article/uninstall-microsoft-teams-3b159754-3c26-4952-abe7-57d27f5f4c81) 여러 대상 컴퓨터 또는 사용자로부터 Microsoft Teams를 정리하기 위해 Microsoft Teams 배포 [정리를 참조합니다.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

공유 컴퓨터, RDS(원격 데스크톱 서비스) 또는 VDI(가상 데스크톱 인프라)를 사용하는 경우 Microsoft Teams를 사용하여 공유 컴퓨터 및 VDI 환경을 [참조하세요.](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams) Mac용 Office를 사용하는 경우 [Mac에서 Microsoft Teams 설치를 참조합니다.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)

**참고:** Teams를 설치한 후 [](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) 약 2주마다 새로운 기능 및 품질 업데이트로 자동으로 업데이트됩니다. 