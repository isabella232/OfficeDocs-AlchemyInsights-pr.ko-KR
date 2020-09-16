---
title: 워크플로 전자 메일이 전송 되지 않음
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
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748995"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>SharePoint 목록 또는 라이브러리에 대해 워크플로 전자 메일이 전송 되지 않음

1. 워크플로의 전자 메일은 모든 사용자 또는 특정 사용자 에게만 전송 되지 않거나, **전자 메일 메시지를 보낼 수 없다는 오류가 표시 됩니다. 전자 메일에 올바른 받는 사람이 있는지 확인 하세요.**

    해당 사이트 모음의 **모든** 사용자 권한 그룹 (사용자 정보 목록)에 사용자가 있는지 확인 합니다.  직접 URL 예제: https:// <tenant> /sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx? MembershipGroupId = 0

    - 사용자가 없는 경우 사용자가 페이지에 로그인 되어 있는지 확인 합니다. 
    - 외부 사용자 인 경우 초대가 수락 되었는지 확인 합니다.
    - 사용자가 사용 권한 그룹에 있는 경우 전자 메일 주소가 올바른지 확인 합니다.
    - 사용자의 전자 메일 주소가 여기에서 설정 되어 있지 않으면 해당 사용자에 대 한 샘플 알림을 만들어 SharePoint의 사용자 프로필에서이 사이트 모음으로 해당 사용자 계정을 강제로 동기화 합니다.
 
2. 워크플로의 전자 메일은 사이트 모음 관리자에 게 전송 되 고 다른 사용자에 게는 전달 되지 않으며 ** <span>https:</span>/client.xvc.sp.utilities.utility.sendemail에 사용할 수**없는 것으로 표시 됩니다 _vti_bin.
 

    [SharePoint 그룹에 전자 메일을 보낼 때 액세스 거부](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)를 참조 하세요.

    또한 **제한 된 액세스 사용자 권한 잠금 모드** 사이트 모음 기능이 활성화 되어 있지 않은지 확인 합니다.


## <a name="related-topics"></a>관련 항목
SharePoint Online에서 Microsoft Flow를 시도 하 고 싶으십니까?
- [흐름 만들기](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint 및 흐름](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


