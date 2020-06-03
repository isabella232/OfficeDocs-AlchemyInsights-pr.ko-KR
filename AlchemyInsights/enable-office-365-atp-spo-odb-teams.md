---
title: SharePoint, OneDrive 및 Microsoft 팀에 Office 365 ATP 사용
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506924"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="cc5f9-102">SharePoint Online, OneDrive 및 Microsoft 팀에 Office 365 Advanced Threat Protection 사용</span><span class="sxs-lookup"><span data-stu-id="cc5f9-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="cc5f9-103">https://protection.office.com으로 이동하여 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="cc5f9-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="cc5f9-104">**위협 관리**  >  **정책**  >  **안전한 첨부 파일**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="cc5f9-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="cc5f9-105">**SharePoint, OneDrive 및 Microsoft 팀에 대해 ATP 설정을**선택 하 고 **저장**을 클릭 합니다.</span><span class="sxs-lookup"><span data-stu-id="cc5f9-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="cc5f9-106">는 전역 관리자 또는 SharePoint Online 관리자는 **DisallowInfectedFileDownload** 매개 변수를 *true*로 설정 하 여 [set-spotenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet을 실행 합니다.</span><span class="sxs-lookup"><span data-stu-id="cc5f9-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="cc5f9-107">는 검색 된 파일에 대 한 [경고를 설정](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) 합니다.</span><span class="sxs-lookup"><span data-stu-id="cc5f9-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="cc5f9-108">ATP는 SharePoint Online, OneDrive 또는 Microsoft 팀의 모든 단일 파일을 검색 합니다.</span><span class="sxs-lookup"><span data-stu-id="cc5f9-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="cc5f9-109">파일은 공유 및 게스트 활동 이벤트를 사용 하는 프로세스 및 악의적인 파일을 식별 하기 위한 스마트 추론 및 위협 신호로 함께 비동기적으로 검색 됩니다.</span><span class="sxs-lookup"><span data-stu-id="cc5f9-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="cc5f9-110">[SharePoint, OneDrive 및 Microsoft 팀에 대 한 ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="cc5f9-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>