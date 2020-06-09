---
title: 독립 실행형 또는 기존 Office 설치를 사용 하 여 팀 배포
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 5ec5277a758fc5171c846266787c2fbcf751f21c
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/09/2020
ms.locfileid: "44617901"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a><span data-ttu-id="00c54-102">독립 실행형 또는 기존 Office 설치를 사용 하 여 팀 배포</span><span class="sxs-lookup"><span data-stu-id="00c54-102">Deploying Teams as standalone or with new or existing Office installations</span></span>

<span data-ttu-id="00c54-103">Microsoft 팀은 이제 엔터프라이즈 용 Microsoft 365 앱, Microsoft 365 Apps 및 Mac 용 Office의 ***새 설치*** 과정에 포함 됩니다.</span><span class="sxs-lookup"><span data-stu-id="00c54-103">Microsoft Teams is now included as part of ***new installations*** of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span> <span data-ttu-id="00c54-104">자세한 내용은 [Microsoft 팀이 Office의 새 설치에 포함 될 때 시작 되는 시기](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps) 를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="00c54-104">For more information, see [When will Microsoft Teams start being included with new installations of Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)</span></span>

<span data-ttu-id="00c54-105">또한 현재 채널의 버전 1906 부터는 기존 설치를 최신 버전으로 업데이트할 때 Windows를 실행 하는 장치에 대 한 Microsoft 365 앱 (Microsoft 365 앱)의 ***기존 설치에*** 팀이 추가 됩니다.</span><span class="sxs-lookup"><span data-stu-id="00c54-105">Additionally, starting with Version 1906 in Current Channel , Teams will be ***added to existing installations*** of Microsoft 365 Apps for enterprise (and Microsoft 365 Apps for business) on devices running Windows when you update your existing installation to the latest version.</span></span> <span data-ttu-id="00c54-106">자세한 내용은 [Office의 기존 설치에 대 한](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps) 자세한 내용을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="00c54-106">For more information, see [What about existing installations of Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)</span></span>

> [!NOTE]
> <span data-ttu-id="00c54-107">이 롤아웃 일정을 기다리지 않으려면 [다음 지침을 수행](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)하 여 사용자에 대 한 독립 실행형으로 팀을 배포   하거나 사용자가 직접 팀을 설치 하도록 할 수 있습니다  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .</span><span class="sxs-lookup"><span data-stu-id="00c54-107">If you don't want to wait for this rollout schedule, you can deploy Teams as standalone for your users by [following these instructions](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) or you can have your users install Teams for themselves from [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads).</span></span>

<span data-ttu-id="00c54-108">조직이 팀을 배포할 준비가 되지 않은 경우 [신규](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) 또는 [기존](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) Office 설치에서 ***팀을 제외*** 하기 위해 수행할 수 있는 단계를 제공 합니다.</span><span class="sxs-lookup"><span data-stu-id="00c54-108">If your organization isn't ready to deploy Teams, we have the steps you can take to ***exclude Teams*** from [new](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) or [existing](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) installations of Office.</span></span> <span data-ttu-id="00c54-109">팀을 설치 하려고 하지만 사용자가 설치 된 후에 자동으로 시작 되지 않도록 하려면 [설치 후에 Microsoft 팀이 자동으로 시작 되지 못하도록](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)합니다 .를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="00c54-109">If you want Teams to be installed, but don't want Teams to start automatically for the user after it's installed, see [Prevent Microsoft Teams from starting automatically after installation](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).</span></span>

<span data-ttu-id="00c54-110">Windows를 실행 하는 장치에서 ***팀을 제거*** 하려면 [Microsoft 팀 제거](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="00c54-110">To ***uninstall Teams*** from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="00c54-111">여러 대상 컴퓨터나 사용자 로부터 Microsoft 팀을 정리 하려면 [Microsoft 팀 배포 정리](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="00c54-111">To cleanup Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>

<span data-ttu-id="00c54-112">공유 컴퓨터, RDS (원격 데스크톱 서비스) 또는 VDI (가상 데스크톱 인프라)를 사용 하는 경우에는 [공유 컴퓨터 및 vdi 환경을 Microsoft 팀과 함께](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="00c54-112">If you're using shared computers, Remote Desktop Services (RDS), or Virtual Desktop Infrastructure (VDI), see [Shared computer and VDI environments with Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).</span></span>

<span data-ttu-id="00c54-113">Mac 용 Office를 사용 하는 경우에 [는 mac에서 Microsoft 팀 설치](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="00c54-113">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>

> [!NOTE]
> <span data-ttu-id="00c54-114">팀이 설치 된 후에는 새로운 기능과 품질 업데이트를 통해 약 2 주 동안 [자동으로 업데이트](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) 됩니다.</span><span class="sxs-lookup"><span data-stu-id="00c54-114">After Teams is installed, it's [automatically updated](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) approximately every two weeks with new features and quality updates.</span></span> 