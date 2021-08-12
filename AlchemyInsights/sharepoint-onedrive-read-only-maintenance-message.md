---
title: Read-Only 사용하려고 할 때 유지 관리 메시지에 대한 SharePoint OneDrive
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
ms.openlocfilehash: edcdea2f5c0647b92c230dd1d86549173e72997fc885195cde688b3b17710a2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53910552"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Read-Only 사용하려고 할 때 유지 관리 메시지에 대한 SharePoint OneDrive

사용자는 다음  시나리오 중 하나에 대해 SharePoint 또는 OneDrive 메시지에 대한 읽기 전용 메시지를 받을 수 있습니다. 

-   계획되거나 활성 상태인 유지 관리 활동입니다.  메시지 센터로 를 확인하여 해당 메시지를 [확인할 수 있습니다.](https://portal.office.com/adminportal/home#/messagecenter)
-   발생될 수 있는 우선 순위가 높은 활성 서비스 인시던트입니다. 서비스 상태로 확인하여 권고/인시던트가 [없는지 검사합니다.](https://portal.office.com/adminportal/home#/servicehealth)
-   30분 미만 동안 지속될 수 있는 서버에서 예기치 않은 이벤트로 인해 발생할 수 있는 사소한 자동 복구 시나리오입니다. 
    
    이러한 사소한 복구에 대한 메시지 센터 또는 서비스 상태 게시물은 없지만 곧 정상으로 돌아와야 합니다.

몇 가지 경우에 위에 나열된 세 가지 시나리오 중 하나에 문제가 있는 것으로 관찰되어 서비스가 복원되지만 사용자 브라우저 캐시가 지워진 것은 아닙니다.

사이트로 가기 전에 브라우저 캐시를 지우어 보십시오.

1. 사용자 Microsoft Edge 에서 설정 **를** 선택한 다음 개인 정보 **및 보안을 선택합니다.**
2. 검색 **지우기에서** **지우기 대상 선택을 선택합니다.**
3. 쿠키 **및 저장된 웹 사이트 데이터 를 선택하고** 지우기 **를 선택합니다.**

>[!Note] 
> 이러한 단계는 Mozilla Firefox 또는 Google Chrome과 같은 다른 브라우저를 사용하는 경우 다를 수 있습니다.

>[!Note] 
> 또 다른 옵션은 새 InPrivate 창에서 SharePoint 사이트 또는 OneDrive 열 수 있습니다.