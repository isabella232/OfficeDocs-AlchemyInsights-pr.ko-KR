---
title: SharePoint 또는 OneDrive에서 액세스 제한
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700461"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>SharePoint 또는 OneDrive에서 액세스 제한

SharePoint Online/OneDrive 서비스에 대 한 액세스를 제한 하는 방법에는 여러 가지가 있습니다. 아래에는 다양 한 액세스 제한 방법이 설명 되어 있습니다. 

**사용 권한 제한**

SharePoint Online 및 비즈니스용 OneDrive에서는 액세스 권한이 있는 그룹/개인 에게만 액세스 권한을 부여 하 여 사이트, 파일 및 폴더와 같은 항목에 대 한 액세스를 제한 합니다.

- [SharePoint 목록 또는 라이브러리에 대 한 사용 권한 사용자 지정](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [SharePoint 사이트 사용 권한 사용자 지정](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [하위 폴더의 사용 권한 변경](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [관리되지 않는 장치에서 액세스 제어](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

SharePoint 또는 전역 관리자로 서, 관리 되지 않는 장치 (예를 들어, Intune에서 하이브리드 AD에 연결 되거나 호환 되지 않는)에 대 한 SharePoint 및 OneDrive 콘텐츠 액세스를 차단 하거나 제한할 수 있습니다.

**네트워크 위치 제한**

IT 관리자는 사용자가 신뢰 하는 정의 된 네트워크 위치를 기반으로 SharePoint 및 OneDrive 리소스에 대 한 액세스를 제어할 수 있습니다. 이를  위치 기반 정책이라고도 합니다. 자세한 내용은 [네트워크 위치를 기반으로 SharePoint Online 및 OneDrive 데이터에 대 한 제어 액세스](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location) 를 참조 하세요.

**사이트 잠금 제한** 

SharePoint Online 내에서는 사이트 모음을 잠글 수 있으므로 아무도 액세스 하지 못합니다. [Get-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState 속성을 사용 하 여 PowerShell 및 [SharePoint Online 관리 셸을](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) 통해이를 설정할 수 있습니다.

**사용자가 사이트 또는 하위 사이트를 만들지 못하도록 제한**

SharePoint 관리자 또는 전역 관리자는 사용자가 자신의 SharePoint 사이트를 만들고 관리 하 고, 만들 수 있는 사이트 종류를 결정 하 고, 사이트의 위치를 지정 하도록 할 수 있습니다. 자세한 내용은 [SharePoint Online에서 사이트 만들기 관리](https://docs.microsoft.com/sharepoint/manage-site-creation) 를 참조 하세요.

