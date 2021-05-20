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
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>온라인, Office 365, SharePoint 및 사용자에 대해 Microsoft Defender를 OneDrive Microsoft Teams

1. https://protection.office.com으로 이동하여 로그인합니다.
2. 위협 **관리 정책**  >  **안전한** 첨부 파일을 선택  >  **합니다.**
3. 에 **대해 Defender 켜기** 를 Office 365, SharePoint, OneDrive 및 Microsoft Teams 를 클릭한 다음 저장을 **클릭합니다.**
4. (권장) 전역 관리자 또는 SharePoint Online 관리자로서 **DisallowInfectedFileDownload** 매개 변수를 true로 설정하여 [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet을 *실행합니다.*
5. (권장) [검색된 파일에](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) 대한 알림을 설정합니다.

> [!NOTE]
> Microsoft Defender for Office 365 Online, SharePoint, OneDrive 또는 Microsoft Teams. 파일은 공유 및 게스트 활동 이벤트를 사용하는 프로세스를 통해 비동기적으로 검색하고 스마트 휴러틱 및 위협 신호와 함께 악성 파일을 식별합니다. 자세한 [내용은 microsoft Defender에서 Office 365, SharePoint OneDrive 및](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)Microsoft Teams.