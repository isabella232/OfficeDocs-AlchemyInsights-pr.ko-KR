---
title: SharePoint Online, Office 365 및 SharePoint Microsoft Defender를 사용하도록 OneDrive Microsoft Teams
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
ms.openlocfilehash: db79c1d79ddb9bc92f0601ac156e5e41a8ab83cd603556f191d5491cdd5ae2a3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058872"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>SharePoint Online, Office 365 및 SharePoint Microsoft Defender를 사용하도록 OneDrive Microsoft Teams

1. 전역 관리자 또는 보안 관리자 자격 증명을 사용하여 Office 365 및 준수 센터에 [로그인합니다.](https://protection.office.com/)
2. 왼쪽 **창에서 위협** 관리를 선택한 다음 정책 금고  >  [선택합니다.](https://protection.office.com/safeattachment)
3. 에 **대해 Microsoft Defender** 켜기Office 365 SharePoint, OneDrive 및 Microsoft Teams 를 선택한 다음 저장을 **선택합니다.**
    > [!TIP]
    >
    > - 전역 관리자 또는 SharePoint Online 관리자는 **DisallowInfectedFileDownload** 매개 변수를 *true로* 설정하여 다음 PowerShell cmdlet을 실행합니다. [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [검색된 파일에 대한 경고 설정](https://go.microsoft.com/fwlink/?linkid=2092110)

자세한 내용은 microsoft [Defender for Office 365 for SharePoint,](https://go.microsoft.com/fwlink/?linkid=2092041)OneDrive 및 Microsoft Teams.
