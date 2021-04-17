---
title: Office 설치에서 Teams 제거 또는 제외
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
- "2662"
- "9000660"
ms.openlocfilehash: 2d96d54cb479f5f52cc707d4307cf9cf1e891a01
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827798"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="6a56f-102">신규 또는 기존 Office 설치에서 Teams 제거 또는 제외</span><span class="sxs-lookup"><span data-stu-id="6a56f-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="6a56f-103">Microsoft Teams는 엔터프라이즈용 Microsoft 365 앱, 비즈니스용 Microsoft 365 앱 및 Mac용 Office의 일부로 포함되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6a56f-103">Microsoft Teams is included as part of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span>

- <span data-ttu-id="6a56f-104">Office 배포 [도구를 사용하여](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) 새 Office 설치에서 Teams를 제외합니다.</span><span class="sxs-lookup"><span data-stu-id="6a56f-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="6a56f-105">Windows를 *실행하는* 장치에서 Teams를 제거하려면 [Microsoft Teams 제거를 참조하세요.](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)</span><span class="sxs-lookup"><span data-stu-id="6a56f-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="6a56f-106">여러 대상 컴퓨터 또는 사용자로부터 Microsoft Teams를 정리하기 위해 Microsoft Teams 배포 [정리를 참조합니다.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)</span><span class="sxs-lookup"><span data-stu-id="6a56f-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="6a56f-107">[PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) 옵션을 사용하여 Microsoft Teams가 Office에 자동으로 설치되지 않도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="6a56f-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="6a56f-108">Teams를 설치하기 전에 [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) 옵션을 사용하여 설치 후 Microsoft Teams가 자동으로 시작되지 않도록 합니다. </span><span class="sxs-lookup"><span data-stu-id="6a56f-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="6a56f-109">Mac용 Office를 사용하는 경우 [Mac에서 Microsoft Teams 설치를 참조합니다.](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)</span><span class="sxs-lookup"><span data-stu-id="6a56f-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>