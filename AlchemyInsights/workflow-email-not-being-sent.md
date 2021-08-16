---
title: 워크플로 전자 메일이 전송되지 않습니다.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 2caf8e0878da0049667d9a19f4488eaec4b9327fbf36be7d29dbf4b7a9c89158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072526"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>워크플로 전자 메일이 SharePoint 라이브러리에 대해 전송되지 않습니다.

1. 워크플로의 전자 메일이 일부 사용자나 특정 사용자에게만 전송되지 않습니다. 또는 전자 메일 메시지를 보낼 수 **없습니다.** 전자 메일에 유효한 받는 사람이 있는지 확인

    해당 사이트 모음에 대한 **모든** 사용자 권한 그룹(사용자 정보 목록)에 사용자가 존재하는지 선택합니다.  샘플 직접 URL: <tenant> https:// .sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx? MembershipGroupId=0

    - 사용자가 존재하지 않는 경우 사용자가 페이지에 로그인해야 합니다. 
    - 외부 사용자인 경우 초대를 수락해야 합니다.
    - 사용자가 사용 권한 그룹에 있는 경우 전자 메일 주소가 올바른지 확인합니다.
    - 여기서 사용자 전자 메일 주소가 설정되지 않은 경우 해당 사용자에 대한 샘플 알림을 만들어 사용자 프로필에서 이 사이트 모음으로 SharePoint 합니다.
 
2. 워크플로의 전자 메일은 사이트 모음 관리자에게 전송되지만 다른 사용자에게는 전송되지 않습니다. **<span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail** 오류가 표시됩니다.
 

    메일 그룹으로 전자 메일을 보낼 때 [액세스가 SharePoint 참조하세요.](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)

    또한 제한된 액세스  사용자 권한 잠금 모드 사이트 모음 기능이 활성화되어 있지 않은지도 확인해야 합니다.


## <a name="related-topics"></a>관련 항목
온라인에서 Microsoft Flow SharePoint 싶나요?
- [사용자 Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint 및 Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


