---
title: Office 설치에서 팀을 제거 하거나 제외 합니다.
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2662"
- "9000660"
ms.openlocfilehash: 22d69db749671afdfe7a809d1bc598e2ad1891d8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658227"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="2296f-102">새 또는 기존 Office 설치에서 팀을 제거 하거나 제외 합니다.</span><span class="sxs-lookup"><span data-stu-id="2296f-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="2296f-103">Microsoft 팀은 microsoft 365 앱 (비즈니스용 microsoft 365 Apps 및 Office for Mac)의 일부로 포함 되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2296f-103">Microsoft Teams is included as part of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span>

- <span data-ttu-id="2296f-104">[Office 배포 도구](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) 를 사용 하 여 새 office 설치에서 팀을 제외 합니다.</span><span class="sxs-lookup"><span data-stu-id="2296f-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="2296f-105">Windows를 실행 하는 장치에서 팀을 *제거* 하려면 [Microsoft 팀 제거](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="2296f-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="2296f-106">여러 대상 컴퓨터나 사용자 로부터 Microsoft 팀을 정리 하려면 [Microsoft 팀 배포 정리](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="2296f-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="2296f-107">Microsoft 팀이 Office와 함께 자동으로 설치 하지 못하도록 하려면 [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) 옵션을 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="2296f-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="2296f-108">Microsoft 팀이 설치 후 자동으로 시작 되지 않도록 하려면 *팀이 설치 되기 전에* [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) 옵션을 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="2296f-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="2296f-109">Mac 용 Office를 사용 하는 경우에 [는 mac에서 Microsoft 팀 설치](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="2296f-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>