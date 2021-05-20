---
title: 사용자 Office 365, SharePoint 및 OneDrive ATP를 사용하도록 Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543934"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="4fb38-102">온라인, Office 365, SharePoint 및 사용자에 대해 Microsoft Defender를 OneDrive Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="4fb38-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="4fb38-103"> https://protection.office.com으로 이동하여 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="4fb38-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="4fb38-104">위협 **관리 정책**  >  **안전한** 첨부 파일을 선택  >  **합니다.**</span><span class="sxs-lookup"><span data-stu-id="4fb38-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="4fb38-105">에 **대해 Defender 켜기** 를 Office 365, SharePoint, OneDrive 및 Microsoft Teams 를 클릭한 다음 저장을 **클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="4fb38-105">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="4fb38-106">(권장) 전역 관리자 또는 SharePoint Online 관리자로서 **DisallowInfectedFileDownload** 매개 변수를 true로 설정하여 [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet을 *실행합니다.*</span><span class="sxs-lookup"><span data-stu-id="4fb38-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="4fb38-107">(권장) [검색된 파일에](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) 대한 알림을 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="4fb38-107">(Recommended) [Set up alerts](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="4fb38-108">Microsoft Defender for Office 365 Online, SharePoint, OneDrive 또는 Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="4fb38-108">Microsoft Defender for Office 365 will not scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="4fb38-109">파일은 공유 및 게스트 활동 이벤트를 사용하는 프로세스를 통해 비동기적으로 검색하고 스마트 휴러틱 및 위협 신호와 함께 악성 파일을 식별합니다.</span><span class="sxs-lookup"><span data-stu-id="4fb38-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="4fb38-110">자세한 [내용은 microsoft Defender에서 Office 365, SharePoint OneDrive 및](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="4fb38-110">See [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>