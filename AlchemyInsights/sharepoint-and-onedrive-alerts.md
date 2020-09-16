---
title: SharePoint 및 OneDrive 알림 받기의 지연
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 27cc744bc57f1c18649e05c5b0df3b315c9c0201
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727249"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>SharePoint 및 OneDrive 알림 받기의 지연

- 먼저 전자 메일에서 정크 또는 스팸 폴더를 확인 합니다.
- **여러 파일 또는 라이브러리의 모든 알림이 지연 된**경우 [서비스 상태 대시보드](https://portal.office.com/adminportal/home?ref=/servicehealth) 를 방문 하 여 SharePoint 또는 Exchange에서 발생할 수 있는 모든 권고/사고를 확인 합니다. 이 문제는 Exchange를 통한 전자 메일의 SharePoint 알림 기능 또는 지연에 있을 수 있습니다. 또한 다른 전자 메일이 배달 되는지 여부도 확인 합니다 (그렇지 않은 경우 Exchange 지연에 문제가 있을 수 있음).
- **특정 파일이 나 라이브러리의 개별 알림이 배달 되지**않으면 삭제 하 고 다시 만듭니다. 경고를 다시 만들려면 [SharePoint 알림 관리, 보기 또는 삭제](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) 를 참조 하세요.

> [!NOTE]
> - 메일 그룹에 알림을 보낼 수 없습니다. 보안 및 O365 그룹만 지원 됩니다.
> - 경고 전자 메일 템플릿은 사용자 지정할 수 없습니다. 이러한 사항을 구현 하려면 Microsoft Flow 또는 SharePoint Designer 워크플로를 사용 해야 합니다.
