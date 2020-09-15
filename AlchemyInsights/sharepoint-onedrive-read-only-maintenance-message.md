---
title: SharePoint 또는 OneDrive를 사용 하려고 할 때 유지 관리 메시지에 대 한 읽기 전용
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670838"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>SharePoint 또는 OneDrive를 사용 하려고 할 때 유지 관리 메시지에 대 한 읽기 전용

사용자는 다음 시나리오 중 하나에 대해 SharePoint 또는 OneDrive를 사용 하려고 할 때 **유지 관리 메시지에 대 한 읽기 전용** 을 받을 수 있습니다. 

-   계획 된 또는 활성 유지 관리 활동  [메시지 센터](https://portal.office.com/adminportal/home#/messagecenter)를 탐색 하 여 확인 합니다.
-   발생할 수 있는 높은 우선 순위의 활성 서비스 인시던트 [서비스 상태](https://portal.office.com/adminportal/home#/servicehealth)를 탐색 하 여 모든 권고/인시던트를 확인 합니다.
-   서버에 대 한 예기치 않은 이벤트 (30 분 미만)로 인해 발생할 수 있는 사소한 자동 복구 복구 시나리오입니다. 
    
    이러한 사소한 복구를 위한 메시지 센터 또는 서비스 상태 게시물은 제공 되지 않지만 곧 정상적으로 백업 해야 합니다.

위의 세 가지 시나리오 중 하나에 문제가 발생 하 여 서비스를 복원 했지만 사용자 브라우저 캐시가 지워지지 않은 경우도 있습니다.

사이트를 탐색 하기 전에 브라우저 캐시를 지워야 합니다.

1. Microsoft Edge 브라우저에서 **설정을**선택한 다음 **개인 정보 및 보안**을 선택 합니다.
2. **검색 지우기**에서 **지우려는 작업**선택을 선택 합니다.
3. **쿠키 및 저장 된 웹 사이트 데이터**를 선택 하 고 **지우기를**선택 합니다.

>[!Note] 
> Mozilla Firefox 또는 Google Chrome과 같은 다른 브라우저를 사용 하는 경우에는 이러한 단계가 다를 수 있습니다.

>[!Note] 
> 또 다른 옵션으로는 SharePoint 사이트 또는 OneDrive를 새 InPrivate 창에서 열 수 있습니다.