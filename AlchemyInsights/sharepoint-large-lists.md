---
title: SharePoint 대규모 목록
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 1bc891a912c6753ea6c85d7d4b2a5d802080bd5c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720139"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a>SharePoint에서 큰 목록 및 라이브러리에 대 한 작업

SharePoint 목록 및 라이브러리에는 최대 3000만 개의 항목이 포함 될 수 있지만, 항목이 5000 개를 초과 하면 작업을 수행 하려고 할 때 목록 보기 임계값 오류가 표시 될 수 있습니다. 이 임계값은 서비스의 성능을 유지하기 위해 설정됩니다. 변경할 수 없습니다. 이 임계값을 초과 하지 않도록 하려면 다음을 수행 합니다.

**최신 사용**

최신 환경에서 가장 잘 작동 하는 많은 항목이 표시 되는 보기 클래식 환경에서 발생할 수 있는 오류를 방지 하려면 [최신 환경을 사용](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) 합니다.

**인덱스 추가**

인덱스가 없는 열을 기준으로 필터링 하거나 정렬 하면 오류 메시지가 표시 될 수 있습니다. [설정] 메뉴의 **목록 설정** 에서 수동으로 [인덱스를 추가한](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) 다음 **인덱싱된 열**을 추가 합니다.

**목록 보기 편집**

큰 목록으로 작업할 때 오류가 발생 하는 경우 [목록 보기를 편집](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372)합니다.

다음 네 가지 변경 사항으로 인해 목록 보기 임계값 오류가 제거 됩니다. 네 가지 사항을 모두 변경 하 여 모든 오류를 제거 합니다. 여전히 오류가 표시 되는 경우 [큰 목록 및 라이브러리 관리](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59)를 선택 합니다.

1. 양쪽에서 **열을 기준으로 첫 번째 정렬** **안** 을 선택한 **다음 열을 기준으로 정렬**합니다.
2. **첫 번째 그룹** **둘 다에서 열을 선택 하** 고 열을 **기준으로 그룹화**합니다.
3. **요약** 섹션에서 모든 열에 대해 아무것도 선택 하지 **않습니다** .
4. **열** 섹션에 표시할 열을 하나만 제외 하 고 모두 선택 취소 합니다.

