---
title: 콘텐츠가 검색 결과에 SharePoint 나타나지 않습니다.
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: ca03c31def64e43935d734a17735b10373e5ca85b5f4ea0f0e886b9ea39884cd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54081616"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>콘텐츠가 검색 결과에 SharePoint 나타나지 않습니다.

예상 콘텐츠가 검색 결과에 나타나지 않는 경우 다음 문제 해결 단계를 따릅니다.
  
1. 예상된  콘텐츠가 포함된 사이트가 검색 결과에 콘텐츠를 표시하도록 설정되어 있는지 검사합니다. 검색 결과에 사이트에 콘텐츠 [표시의 단계를 따릅니다.](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)

2. 예상된 **콘텐츠가** 포함된 목록 또는 라이브러리가 검색 결과에 콘텐츠를 표시하도록 설정되어 있는지 검사합니다.  검색 결과에 목록 또는 라이브러리의 콘텐츠 [표시의 단계를 따릅니다.](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)

3. 페이지, 문서 또는 사용자 지정 페이지 레이아웃이 주 버전으로 게시되어 **있는지 확인하십시오.** 검색의 3단계를 수행해도 온라인 에서 모든 결과가 [SharePoint 않습니다.](https://go.microsoft.com/fwlink/?linkid=874525)

4. 사용자에게 콘텐츠를 **볼** 수 있는 권한이 있는지 확인 Understanding permission [levels in SharePoint.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)
    
5. 새 관리 속성을 추가하거나, 관리 속성을 편집하거나, 관리 속성을 제거하여 검색 schema를 변경한 경우 크롤링 및 다시 인덱싱을 요청해야 합니다. **사이트,** 라이브러리 또는 목록의 크롤링 및 다시 인덱싱을 수동으로 요청의 단계에 따라 콘텐츠를 [다시 인덱싱합니다.](https://docs.microsoft.com/sharepoint/crawl-site-content) 이 경우 시간이 걸릴 수 있습니다. 결과를 다시 확인하기 전에 24시간을 기다릴 수 있습니다.

자세한 내용은 사이트의 콘텐츠를 검색 가능하도록 설정을 [참조하세요.](https://docs.microsoft.com/sharepoint/make-site-content-searchable) 
  
