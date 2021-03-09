---
title: SharePoint Online, OneDrive 및 Microsoft Teams용 Office 365용 Microsoft Defender 사용
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50552425"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="9622c-102">SharePoint Online, OneDrive 및 Microsoft Teams용 Office 365용 Microsoft Defender 사용</span><span class="sxs-lookup"><span data-stu-id="9622c-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive and Microsoft Teams</span></span>

1. <span data-ttu-id="9622c-103">전역 관리자 또는 보안 관리자 자격 증명을 사용하여 Office 365 보안 및 준수 [센터에 로그인합니다.](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="9622c-103">Using your global admin or security admin credentials, log in to the [Office 365 Security and Compliance Center](https://protection.office.com/).</span></span>
2. <span data-ttu-id="9622c-104">왼쪽 **창에서 위협** 관리를 선택한 다음 정책 안전한 **첨부**  >  [파일을 선택합니다.](https://protection.office.com/safeattachment)</span><span class="sxs-lookup"><span data-stu-id="9622c-104">Select **Threat management** in the left pane, and then select **Policy** > [Safe attachments](https://protection.office.com/safeattachment).</span></span>
3. <span data-ttu-id="9622c-105">**SharePoint, OneDrive 및 Microsoft Teams용 Office 365용 Microsoft Defender** 켜기 를 선택하고 저장을 **선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="9622c-105">Select **Turn on Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then select **Save**.</span></span>
    > [!TIP]
    >
    > - <span data-ttu-id="9622c-106">전역 관리자 또는 SharePoint Online 관리자는 **DisallowInfectedFileDownload** 매개 변수를 *true로* 설정하여 다음 PowerShell cmdlet을 실행합니다. [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span><span class="sxs-lookup"><span data-stu-id="9622c-106">As a global admin or a SharePoint Online admin, run the following PowerShell cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span></span>
    > - [<span data-ttu-id="9622c-107">검색된 파일에 대한 경고 설정</span><span class="sxs-lookup"><span data-stu-id="9622c-107">Set up alerts for detected files</span></span>](https://go.microsoft.com/fwlink/?linkid=2092110)

<span data-ttu-id="9622c-108">자세한 내용은 [SharePoint, OneDrive 및 Microsoft Teams용 Office 365용 Microsoft Defender를 참조하세요.](https://go.microsoft.com/fwlink/?linkid=2092041)</span><span class="sxs-lookup"><span data-stu-id="9622c-108">For more information, see [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).</span></span>
