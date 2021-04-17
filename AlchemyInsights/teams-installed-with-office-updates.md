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
# <a name="microsoft-teams-installed-with-office-updates"></a><span data-ttu-id="3536b-102">Office 업데이트와 함께 설치된 Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="3536b-102">Microsoft Teams installed with Office updates</span></span>

<span data-ttu-id="3536b-103">Microsoft Teams는 엔터프라이즈용  Microsoft 365 앱, 비즈니스용 Microsoft 365 앱 및 Mac용 Office의 새 설치의 일부로 포함됩니다.</span><span class="sxs-lookup"><span data-stu-id="3536b-103">Microsoft Teams is included as part of ***new installations*** of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span> <span data-ttu-id="3536b-104">자세한 내용은 언제 Microsoft Teams가 Office의 새 설치에 포함 [되나요?를 참조하세요.](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)</span><span class="sxs-lookup"><span data-stu-id="3536b-104">For more information, see [When will Microsoft Teams start being included with new installations of Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)</span></span>

<span data-ttu-id="3536b-105">또한 현재 채널의 버전 1906부터는 기존 설치를  최신 버전으로 업데이트할 때 Windows를 실행하는 장치에서 엔터프라이즈용 Microsoft 365 앱(및 비즈니스용 Microsoft 365 앱)의 기존 설치에 Teams가 점진적으로 추가됩니다.</span><span class="sxs-lookup"><span data-stu-id="3536b-105">Additionally, starting with Version 1906 in Current Channel , Teams will gradually be added to ***existing installations*** of Microsoft 365 Apps for enterprise (and Microsoft 365 Apps for business) on devices running Windows when you update your existing installation to the latest version.</span></span> <span data-ttu-id="3536b-106">자세한 내용은 Office의 기존 설치에 대한 [정보를 참조하세요.](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)</span><span class="sxs-lookup"><span data-stu-id="3536b-106">For more information, see [What about existing installations of Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)</span></span>

<span data-ttu-id="3536b-107">**참고:** 이 출시 일정을 기다리지 않는 경우 다음 지침에 따라 사용자를 위한 독립 [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)실행형으로 Teams를 배포하거나 사용자가 에서 Teams를 직접 설치하도록 할 수 https://teams.microsoft.com/downloads 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3536b-107">**Note:** If you don't want to wait for this rollout schedule, you can deploy Teams as standalone for your users by [following these instructions](https://docs.microsoft.com/MicrosoftTeams/msi-deployment), or you can have your users install Teams for themselves from https://teams.microsoft.com/downloads.</span></span>

<span data-ttu-id="3536b-108">조직에서 Teams를 배포할 준비가 되어 있지 않은 [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) 경우 [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) Office의 신규 또는 기존 설치에서 ***Teams를*** 제외할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3536b-108">If your organization isn't ready to deploy Teams, you can ***exclude Teams*** from [new](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) or [existing](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) installations of Office.</span></span> <span data-ttu-id="3536b-109">Teams를 설치하겠지만 Teams가 설치된 후 사용자를 위해 자동으로 시작하지 않도록 하려는 경우 설치 후 Microsoft Teams가 자동으로 시작되지 않도록 방지를 [참조합니다.](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)</span><span class="sxs-lookup"><span data-stu-id="3536b-109">If you want Teams to be installed, but don't want Teams to start automatically for the user after it's installed, see [Prevent Microsoft Teams from starting automatically after installation](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).</span></span>

<span data-ttu-id="3536b-110">Windows를 실행하는 장치에서 ***Teams를*** 제거하려면 [Microsoft Teams 제거를 참조하세요.](https://support.office.com/article/uninstall-microsoft-teams-3b159754-3c26-4952-abe7-57d27f5f4c81)</span><span class="sxs-lookup"><span data-stu-id="3536b-110">To ***uninstall Teams*** from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/uninstall-microsoft-teams-3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="3536b-111">여러 대상 컴퓨터 또는 사용자로부터 Microsoft Teams를 정리하기 위해 Microsoft Teams 배포 [정리를 참조합니다.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)</span><span class="sxs-lookup"><span data-stu-id="3536b-111">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment cleanup](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>

<span data-ttu-id="3536b-112">공유 컴퓨터, RDS(원격 데스크톱 서비스) 또는 VDI(가상 데스크톱 인프라)를 사용하는 경우 Microsoft Teams를 사용하여 공유 컴퓨터 및 VDI 환경을 [참조하세요.](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)</span><span class="sxs-lookup"><span data-stu-id="3536b-112">If you're using shared computers, Remote Desktop Services (RDS), or Virtual Desktop Infrastructure (VDI), see [Shared computer and VDI environments with Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).</span></span> <span data-ttu-id="3536b-113">Mac용 Office를 사용하는 경우 [Mac에서 Microsoft Teams 설치를 참조합니다.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)</span><span class="sxs-lookup"><span data-stu-id="3536b-113">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>

<span data-ttu-id="3536b-114">**참고:** Teams를 설치한 후 [](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) 약 2주마다 새로운 기능 및 품질 업데이트로 자동으로 업데이트됩니다.</span><span class="sxs-lookup"><span data-stu-id="3536b-114">**Note:** After Teams is installed, it's [automatically updated](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) approximately every two weeks with new features and quality updates.</span></span> 