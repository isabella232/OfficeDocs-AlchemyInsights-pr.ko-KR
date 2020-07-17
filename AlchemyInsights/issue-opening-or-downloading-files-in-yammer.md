---
title: Yammer에서 파일 열기 혹은 다운로드 문제
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45146817"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Yammer에서 파일 열기 혹은 다운로드 문제

클래식 Yammer는 메시지와 그룹에 파일을 업로드하는데 다양한 옵션을 지원합니다. 네트워크 구성에 따라 파일은 기본적으로 SharePoint의 저장소로 설정됩니다.

클래식 Yammer에서 사용할 수 있는 일부 옵션이 새로운 Yammer 파일 피커에서 아직 지원 되지 않습니다. 향후 업데이트에는 추가 기능이 추가 될 것입니다. 자세한 내용은 [Yammer 대화 게시글에 파일 혹은 이미지 첨부](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8)를 참조하세요.

**파일을 열거나 다운로드할 수 없음**  

파일은 Yammer에 업로드 되지만 SharePoint Online의 파일에 연결 됩니다. 문제를 해결 하려면 먼저 파일의 위치를 확인 해야 합니다. 파일을 Yammer에 업로드 한 경우에는 *. yammer.com URL이 있습니다. 필수 URL과 IP 주소가 차단 되지 않았는지 확인합니다. 자세한 내용은 [Yammer에서 하드 코드 된 IP 주소 사용은 권장되지 않음](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592) 블로그 게시물을 참조하세요.

전역 관리자인 사용자가 파일을 다운로드할 수 있는지 확인합니다. 파일이 비공개인 경우 비공개 콘텐츠 모드를 사용 해야 할 수 있습니다. 자세한 내용은 [Yammer에서 개인 콘텐츠 모니터링](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content)을 참조하세요.  

**Yammer 네트워크 수준 게스트 및 SharePoint Online의 파일**  

[Yammer의 네트워크 수준 게스트](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) Azure AD B2B를 사용하지 않고 Yammer 서비스 내부에 있기 때문에 SharePoint에서 Yammer 파일에 액세스 할 수 없습니다. 해당 ID를 사용하여 SharePoint Online에서 문서 라이브러리에 액세스할 수 있는 외부 AAD B2B 사용자를 만듭니다. Yammer에서 미래 Azure AD B2B 게스트 지원에 대한 자세한 내용은 [Yammer 미리보기에서 B2B 게스트 지원 - 고객 약관 및 FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer)를 참조하세요.