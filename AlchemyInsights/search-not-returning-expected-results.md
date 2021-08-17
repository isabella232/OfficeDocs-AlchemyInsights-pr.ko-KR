---
title: 1491-search-not-returning-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 846034d68a59d053cbe37aeba3a75e20a60786fd7ff24106964229b1deb77608
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052716"
---
# <a name="content-search-not-returning-expected-results"></a>콘텐츠 검색에서 예상된 결과를 반환하지 않습니다.

보안 및 준수 센터에서 콘텐츠 Microsoft 365 & 실행하면 예기치 않은 검색 결과가 표시될 수 있습니다. 검색 결과에 영향을 줄 수 있는 다음을 고려합니다.

- **콘텐츠 위치 및 검색 조건:** 적절한 콘텐츠 위치 및 검색 조건을 선택해야 합니다. 많은 위치의 대규모 검색을 한 경우 여러 검색으로 분할하는 것이 있습니다.

- **부분적으로 인덱싱된 항목:** 사서함에서 부분적으로 인덱싱된 항목이 예상 검색 결과에 포함됩니다. [](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) 그러나 SharePoint 및 OneDrive 사이트의 부분적으로 인덱싱된 항목은 검색 예상에 포함되지 않습니다.

- 검색 **오류:** 많은 수의 사서함(100,000개가 넘는 사서함)을 검색할 때 CS008-009 및 CS012-002와 같은 오류 코드를 사용하여 검색 오류가 발생할 수 있습니다. 이 경우 실패한 콘텐츠 위치에 대한 검색만 다시 시도합니다. 자세한  [내용은 이 문서를](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) 참조하세요.
