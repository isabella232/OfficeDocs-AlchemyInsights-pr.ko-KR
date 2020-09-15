---
title: SharePoint, OneDrive 및 Microsoft 팀에 Office 365 ATP 사용
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
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709913"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>SharePoint Online, OneDrive 및 Microsoft 팀에 Office 365 Advanced Threat Protection 사용

1. https://protection.office.com으로 이동하여 로그인합니다.
2. **위협 관리**  >  **정책**  >  **안전한 첨부 파일**을 선택 합니다.
3. **SharePoint, OneDrive 및 Microsoft 팀에 대해 ATP 설정을**선택 하 고 **저장**을 클릭 합니다.
4. 는 전역 관리자 또는 SharePoint Online 관리자는 **DisallowInfectedFileDownload** 매개 변수를 *true*로 설정 하 여 [set-spotenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet을 실행 합니다.
5. 는 검색 된 파일에 대 한 [경고를 설정](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) 합니다.

> [!NOTE]
> ATP는 SharePoint Online, OneDrive 또는 Microsoft 팀의 모든 단일 파일을 검색 합니다. 파일은 공유 및 게스트 활동 이벤트를 사용 하는 프로세스 및 악의적인 파일을 식별 하기 위한 스마트 추론 및 위협 신호로 함께 비동기적으로 검색 됩니다. [SharePoint, OneDrive 및 Microsoft 팀에 대 한 ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)를 참조 하세요.