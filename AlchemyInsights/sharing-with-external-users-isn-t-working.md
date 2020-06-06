---
title: 외부 사용자와의 공유가 작동 하지 않음
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 9a40f52637bc8aa7894754118f0f862aa6c71fe2
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582781"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>외부 사용자와 SharePoint 콘텐츠를 공유 하는 문제 해결

조직에 대해 외부 공유가 설정 되어 있는지 확인 합니다.
  
1. [ &amp; Microsoft 365 관리 센터에서 서비스 추가 기능 페이지로](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)이동 하 고 **사이트**를 클릭 합니다.
    
2. 설정이 "설정"으로 설정 되어 있는지 확인 합니다. "기존 외부 사용자만"을 선택 하는 경우에는 외부 사용자가 Microsoft 365 관리 센터에 나열 되어 있는지 확인 합니다.
    
사이트에 대 한 외부 공유를 설정 했는지 확인 합니다. 클래식 사이트 모음의 경우 다음을 수행 합니다.
  
1. 새 SharePoint 관리 센터의 왼쪽 창에서 **사이트**를 클릭 합니다.
    
2. 사이트 또는 사이트를 선택 하 고 리본 메뉴에서 **공유**를 클릭 합니다.
    
Microsoft 365 그룹 또는 커뮤니케이션 사이트에 속하는 팀 사이트의 경우:
  
- 조직 차원의 설정에서 로그인이 필요 하지 않은 링크를 사용 하 여 파일을 공유할 수 있는 경우를 제외 하 고 이러한 새 사이트 유형은 조직 전체 설정과 동일한 공유 설정을 갖습니다. 이 경우 사이트는 로그인 하는 신규 및 기존 외부 사용자와의 공유를 허용 합니다. 특정 사이트에 대 한 설정을 변경 하려면 새 SharePoint 관리 센터 또는 PowerShell을 사용 합니다. [자세히 알아보세요](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> 모든 사이트에 대 한 외부 공유 설정은 조직 차원의 설정 보다 더 제한적으로 사용할 수 있지만 조직 전체 설정 보다는 허용이 더 이상 가능 하지 않습니다. 
  

