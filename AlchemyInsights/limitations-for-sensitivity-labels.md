---
title: SharePoint 및 OneDrive의 Office 파일에 대한 민감도 레이블 제한
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12451"
- "9000181"
ms.openlocfilehash: c3a0695dc2aa5f6e56be2235f08c81dbbe7fcea2
ms.sourcegitcommit: 86c95d3f0f268e500b3732243ca85a650b2e7b8f
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53533001"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>SharePoint 및 OneDrive의 Office 파일에 대한 민감도 레이블 제한

SharePoint 및 OneDrive에서 Office 파일에 대한 민감도 레이블을 활성화할 때 다음을 포함하는 요구 사항 및 제한 사항에 유의하세요.

- 파일에 PowerQuery 데이터, 사용자 지정 추가 기능에 의해 저장된 데이터 또는 사용자 지정 XML 부분이 포함된 경우 SharePoint 및 OneDrive는 Office 데스크톱 앱에서 레이블이 지정되고 암호화된 일부 파일을 처리할 수 없습니다.
- SharePoint 및 OneDrive는 AIP(Azure Information Protection) 레이블을 사용하여 이미 암호화한 기존 파일에 민감도 레이블을 자동으로 적용하지 않습니다. 암호화된 파일에 민감도 레이블을 적용하려면: 
    - AIP 레이블이 마이그레이션되어 Microsoft 365 준수 센터에 게시되었는지 확인합니다.
    - 레이블이 지정된 파일을 다운로드한 다음 원래 SharePoint 또는 OneDrive 위치에 업로드합니다.
- 암호화된 문서의 경우 인쇄가 지원되지 않습니다.

제한에 대한 추가 세부 정보는 [SharePoint 및 OneDrive에서 Office 파일에 대한 민감도 레이블 사용](/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations)을 참조하세요.
