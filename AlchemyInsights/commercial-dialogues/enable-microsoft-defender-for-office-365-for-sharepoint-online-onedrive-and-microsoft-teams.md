---
title: 금고 Online, SharePoint 및 OneDrive 첨부 파일에 Microsoft Teams
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
ms.openlocfilehash: 61372075ac8ccf04606a8003b4ec29f89fc048e5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332385"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>금고 Online, SharePoint 및 OneDrive 첨부 파일에 Microsoft Teams

1. 전역 관리자 또는 보안 관리자 자격 증명을 사용하여 Microsoft 365 Defender 포털을 열고 정책 섹션의 정책 & 규칙 위협 금고 정책으로 <https://security.microsoft.com>  \>  \> **이동하십시오.** 

   첨부 파일 **페이지로** 직접 금고 를 <https://security.microsoft.com/safeattachmentv2> 사용하세요.

2. 첨부 **금고 페이지에서** 전역 설정을 **클릭합니다.**
3. 플라이아웃이 나타나면 에 대해 **Microsoft Defender에서** Office 365, SharePoint, OneDrive 및 Microsoft Teams 를 **선택합니다.**

    **팁:** 다음 단계를 수행하여 금고, 파일 및 SharePoint 첨부 OneDrive 보호를 Microsoft Teams.
    - 사용자가 악성 파일을 다운로드하지 못하게 방지하려면 SharePoint `$true` Online PowerShell의 **[Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** cmdlet에서 *DisallowInfectedFileDownload* 매개 변수의 값을 사용합니다. 자세한 내용은 [Use SharePoint Online PowerShell to prevent users from downloading malicious files을 참조하세요.](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files)
    - [검색된 파일에 대한 경고 정책 만들기](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

자세한 내용은 금고, Office 365 및 에 대한 SharePoint 첨부 OneDrive [Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)
