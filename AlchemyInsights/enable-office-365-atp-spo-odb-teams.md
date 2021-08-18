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
ms.openlocfilehash: 2d132101768e0a835d448604d684ec0c735e6628
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332165"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>온라인, Office 365, SharePoint 및 사용자에 대해 Microsoft Defender를 OneDrive Microsoft Teams

1. https://protection.office.com으로 이동하여 로그인합니다.
2. 위협 **관리 정책**  >  **금고**  >  **를 선택 합니다.**
3. 에 **대해 Defender 켜기** 를 Office 365, SharePoint, OneDrive 및 Microsoft Teams 를 클릭한 다음 저장을 **클릭합니다.**
4. (권장) 전역 관리자 또는 SharePoint Online 관리자로서 **DisallowInfectedFileDownload** 매개 변수를 true로 설정하여 [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet을 *실행합니다.*
5. (권장) [검색된 파일에](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) 대한 알림을 설정합니다.

**참고:** microsoft Defender for Office 365 Online, SharePoint, OneDrive 또는 Microsoft Teams. 파일은 공유 및 게스트 활동 이벤트를 사용하는 프로세스를 통해 비동기적으로 검색하고 스마트 휴러틱 및 위협 신호와 함께 악성 파일을 식별합니다. 자세한 [내용은 microsoft Defender에서 Office 365, SharePoint OneDrive 및](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)Microsoft Teams.
