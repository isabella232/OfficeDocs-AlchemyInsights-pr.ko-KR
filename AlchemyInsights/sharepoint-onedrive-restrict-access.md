---
title: 웹 응용 SharePoint 액세스 OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: fc6731d5a7747bb4fc8d6cef1b6ac0045d11917d7f97abbb21eea9613b1b1aa2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093839"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>웹 응용 SharePoint 액세스 OneDrive

여러 가지 방법으로 온라인/SharePoint 서비스에 대한 액세스를 OneDrive 있습니다. 이러한 다양한 액세스 제한 방법은 아래에서 간략하게 설명합니다. 

**사용 권한 제한**

SharePoint Online 및 비즈니스용 OneDrive, 액세스 권한이 있는 그룹/개인에게만 액세스 권한을 부여하여 사이트, 파일 및 폴더와 같은 항목에 대한 액세스를 제한합니다.

- [목록 또는 라이브러리에 대한 SharePoint 사용자 지정](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [SharePoint 사이트 사용 권한 사용자 지정](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [하위 폴더의 사용 권한 변경](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [관리되지 않는 장치에서 액세스 제어](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

SharePoint 또는 전역 관리자는 관리되지 않는 디바이스(Intune에서 하이브리드 AD에 가입되거나 규정을 준수하지 않는 SharePoint 및 OneDrive 콘텐츠에 대한 액세스를 차단하거나 제한할 수 있습니다.

**네트워크 위치 제한**

IT 관리자는 신뢰할 수 있는 정의된 네트워크 위치에 따라 SharePoint OneDrive 리소스에 대한 액세스를 제어할 수 있습니다. 이를 위치 기반 정책이라고도 합니다. 자세한 내용은 네트워크 위치에 따라 SharePoint 온라인 및 OneDrive [액세스 제어를 참조하세요.](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**사이트 잠금 제한** 

SharePoint Online 내에서는 사이트 모음을 잠글 수 있으므로 누구도 액세스할 수 없습니다. 이 설정은 PowerShell [](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) 및 [SharePoint-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState 속성을 사용하여 온라인 관리 셸을 통해 설정됩니다.

**사용자가 사이트 또는 하위 사이트를 만들 수 있도록 제한**

SharePoint 관리자 또는 전역 관리자는 사용자가 자신의 SharePoint 사이트를 만들고 관리하고, 만들 수 있는 사이트 종류를 결정하고, 사이트의 위치를 지정할 수 있습니다. 자세한 내용은 Manage [site creation in SharePoint Online를 참조하세요.](https://docs.microsoft.com/sharepoint/manage-site-creation)

