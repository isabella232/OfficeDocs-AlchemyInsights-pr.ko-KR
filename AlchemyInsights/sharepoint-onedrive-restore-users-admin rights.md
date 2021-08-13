---
title: 사이트 액세스 거부 메시지 비즈니스용 OneDrive 문제 해결
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: fc4a2bd7dcc74f5f05e8b709e4bc3eac6ed445d6e2ea9ede698abbc8667723ce
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957799"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>사이트 액세스 거부 메시지 비즈니스용 OneDrive 문제 해결

이 문제는 사용자가 삭제된 후 UPN(사용자 계정 이름)으로 다시 생성될 때 가장 자주 발생합니다. 새 계정은 다른 PUID(Passport Unique ID) 값을 사용하여 만들어집니다. 사용자가 사이트 모음 또는 사이트 모음에 액세스하는 OneDrive PUID가 잘못되었습니다. 두 번째 시나리오에는 Active Directory OU(조직 구성 단위)와 디렉터리 동기화가 포함됩니다. 사용자가 이미 SharePoint 로그인한 후 다른 OU로 이동하여 SharePoint 경우 이 문제가 발생하게 될 수 있습니다.

1. 이 문제를 해결하기 위해 원본 UPN을 복원해야 합니다( [Restore a user in Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)
2. 원래 사용자를 복원할 수 없는 경우 다음 단계를 사용하여 OneDrive 사이트에서 이전 사용자를 제거해야 합니다. 사용자 정보 목록에서 사용자 [제거.]() 
3. 이 단계를 완료한 후 사용자의 관리자 권한 추가 단계에 따라 OneDrive 사이트에 대한 관리자 권한이 있는지 확인할 [수 OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)

권한 수준에 대한 자세한 내용은 [Understanding permission levels in SharePoint.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)
