---
title: 외부 사용자와의 공유가 작동하지 않습니다.
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 53f6fd009d3dab3cd66d33d9cd248201219caa1605c7a4e7758a5a8d720f68c2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53910372"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>외부 사용자와 SharePoint 공유하는 문제 해결

조직에 대해 외부 공유가 설정되어 있는지 확인:
  
1. 에서 서비스 추가 기능 [ &amp; 페이지로 이동하여](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)Microsoft 365 관리 센터 **를 클릭합니다.**
    
2. 설정이 "켜기"로 설정되어 있는지 확인 "기존 외부 사용자만"을 선택한 경우 외부 사용자가 외부 사용자 목록에 Microsoft 365 관리 센터.
    
사이트에 대해 외부 공유를 설정해야 합니다. 클래식 사이트 모음의 경우:
  
1. 새 SharePoint 관리 센터의 왼쪽 창에서 사이트를 **클릭합니다.**
    
2. 사이트 또는 사이트를 선택하고 리본에서 공유를 **클릭합니다.**
    
Microsoft 365 또는 커뮤니케이션 사이트에 속하는 팀 사이트의 경우:
  
- 이러한 새 사이트 유형은 조직 전체 설정에서 로그인이 필요하지 않은 링크를 사용하여 파일을 공유하는 것을 허용하지 않는 한 조직 전체의 공유 설정과 동일합니다. 이 경우 사이트에서는 로그인하는 새 외부 사용자 및 기존 외부 사용자와의 공유를 허용합니다. 특정 사이트의 설정을 변경하려면 새 SharePoint 관리 센터 또는 PowerShell을 사용하세요. [자세히 알아보기](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> 모든 사이트의 외부 공유 설정은 조직 전체 설정보다 더 제한적일 수 있지만 조직 전체 설정보다는 더 제한적일 수 있습니다. 
  

