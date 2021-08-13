---
title: Yammer에서 이미지 로딩 문제 해결
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6000"
- "9003112"
ms.openlocfilehash: 11315fd84f92251e435320f4550286fb2db4b0128f7ac85c0f79972e3f7fd203
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939241"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a>Yammer에서 이미지 로딩 문제 해결

Yammer에서 사진 및 파일 미리 보기와 관련 된 문제가 발생하면 모든 사용자에게 해당 문제가 발생하는지 여부를 확인하고, 모바일 장치에서 발생하는지, 첨부 파일을 업로드할 때 복사 할 수 있는지 확인하여 문제를 해결합니다.  

**프로필 사진 문제**  

최종 사용자가 Microsoft 365를 통해 Yammer에 로그인하는 경우 프로필 사진을 포함하여 프로필을 변경해야 합니다. 사용자가 프로필 업데이트를 수행할 수 없는 경우 관리자가 사용자를 위해 업데이트 할 수 있습니다. 자세한 내용은 [Office Delve에서 프로필 보기 및 업데이트](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba)를 참조하세요.

프로필 사진을 포함하여 프로필 편집에 대한 자세한 내용은 [Yammer 프로필과 설정 변경](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851)을 참조하세요. 

업데이트 된 프로필 사진은 프로필 속성과 다르게 동기화 됩니다. 사용자가 프로필 사진의 동기화를 시작 하려면 로그인 해야 합니다. 자세한 내용은 [사용자 프로필 사진이 Office 365에서 Yammer로 업데이트 되나요](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer)를 참조하세요.

Yammer의 사용자 수명 주기에 대한 자세한 내용은 [Office 365에서 수명 주기 동안 Yammer 사용자 관리](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle)를 참조하세요.  

Microsoft 365에서 프로필 사진 동기화가 적용 되는 방법에 대한 자세한 내용은 [Microsoft 365에서 프로필 사진 동기화 정보](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a)를 참조 하세요.  

**문서 미리 보기 및 이미지 축소판 그림 문제**  

파일이나 이미지를 Yammer에 게시 할 때 다음 때문에 미리 보기가 표시 되지 않을 수 있습니다. 

- 파일이 손상되어 처리할 수 없습니다.
- 최근에 SharePoint Online에 파일이 업로드 되지 않은 경우 또는 Yammer에 다른 이유로 인해 잘못 된 메타 데이터가 있는 경우
- 미리보기 이미지를 로딩하는데 필요한 URL은 차단됩니다.
- 파일 미리보기는 게시 전에 사용자에 의해 제거 되었습니다.
- 서비스 문제 때문에 미리 보기를 생성할 수 없습니다.

**알림** 링크와 파일 업로드 미리보기가 다르게 작동 할 수 있습니다. 추가 인증이 필요한 인터넷 혹은 링크에서 파일 링크가 올바르게 표시되지 않을 수 있습니다.

자세한 내용은 [Yammer 메시지에 파일 또는 이미지 첨부](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf)를 참조하세요. 