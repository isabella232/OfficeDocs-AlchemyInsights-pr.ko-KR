---
title: 사용자용 추가 기능 Microsoft 365 앱
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: e55d8e5453f60b5993500dae1eb6efce11a8aa1a
ms.sourcegitcommit: d74039304002e526ba6f8ca02e76e4ce7e1aa743
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/30/2021
ms.locfileid: "52107531"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>사용자용 추가 기능 Microsoft 365 앱

중앙 집중식 배포는 조직 내의 사용자 및 그룹에 Office 추가 기능을 배포하는 데 권장되는 방법입니다. 추가 기능을 배포하기 위해 다음 단계를 따르세요.

**참고:** 개별 사용자로 사용할 추가 기능을 Office 프로그램 에서 추가 기능 [보기, 관리 및 설치를 Office 참조합니다.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d) 또한 스토어 추가 기능의 개별 Office 사용하도록 설정되어 있는지 확인합니다. 

1. 환경이 중앙 집중식 배포를 사용하여 추가 기능을 배포하기 위한 요구 사항을 충족하는지 확인합니다. 자세한 내용은 Requirements을 [참조하세요.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements)
2. 통합 **설정** 추가 기능을 배포하려면 Microsoft 365 관리 센터에서 앱  >    >   다운로드로 이동하세요. 

참고: 

- 통합 앱을 사용하려면 관리자에게 전역 관리자 또는 관리자 권한이 Exchange 필요합니다.

- 여러 사용자에게 추가 기능을 배포할 때 개별 사용자 대신 그룹을 사용하여 할당하는 것이 좋습니다. 자세한 내용은 사용자 및 그룹에 추가 기능을 할당할 때 고려 [사항을 참조합니다.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)

- 중앙 집중식 배포는 상위 그룹이 있는 중첩된 그룹 또는 그룹의 사용자를 지원하지 않습니다. 자세한 내용은 사용자 및 그룹 [할당을 참조합니다.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)

- 사용자가 로그인할 수 있도록 Microsoft 365 앱 관리 서비스(GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a')가 사용하도록 설정되어 있는지 확인합니다. 자세한 내용은 앱 속성 [구성을 참조하세요.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)

- 통합 앱을 사용하여 추가 기능을 배포하는 데 문제가 있는 경우 추가 기능을 사용하여 [배포해 보아야 합니다.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)

자세한 내용은 다음을 참조하세요.

[관리 센터에서 추가 기능 배포](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [관리 센터에서 추가 기능 관리](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [중앙 집중식 배포 PowerShell cmdlet을](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 사용하여 추가 기능 관리 
 중앙 Office 센터를 통해 중앙 집중식 배포를 사용하여 Microsoft 365 [추가 기능 게시](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [문제 해결: 사용자가 추가 기능을 볼 수 없습니다.](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [추가 기능을 사용하여 사용자 Office 해결](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)