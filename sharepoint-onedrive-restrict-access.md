---
title: SharePoint 또는 OneDrive에서 액세스 제한
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 5115a8eb6dd9cd25b556353b4f61f10ae4598ff6
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/04/2019
ms.locfileid: "34718227"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>SharePoint 또는 OneDrive에서 액세스 제한

<p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">SharePoint Online/OneDrive 서비스에 대 한 액세스를 제한 하는 방법에는 여러 가지가 있습니다. 아래에는 다양 한 액세스 제한 방법이 설명 되어 있습니다.</span></p> <p><strong style="mso-bidi-font-weight: normal;"><u><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">사용 권한 제한</span></u></strong></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">SharePoint Online 및 비즈니스용 OneDrive에서는 액세스 권한이 있는 그룹/개인 에게만 액세스 권한을 부여 하 여 사이트, 파일 및 폴더와 같은 항목에 대 한 액세스를 제한 합니다.</span></p> <ul> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;"><a href="https://support.office.com/en-us/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782">SharePoint 목록 또는 라이브러리에 대 한 사용 권한 사용자 지정</a></span></li> </ul> <ul> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;"><a href="https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions">SharePoint 사이트 사용 권한 사용자 지정</a></span></li> </ul> <ul> <li><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;"><a href="https://support.office.com/en-us/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6">하위 폴더의 사용 권한 변경</a></span></li> </ul> <p><strong style="mso-bidi-font-weight: normal;"><u><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">관리되지 않는 장치에서 액세스 제어</span></u></strong></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Office 365의 SharePoint 또는 전역 관리자로 서, 관리 되지 않는 장치 (예를 들어, Intune에서 하이브리드 AD에 연결 되거나 호환 되지 않는) <a href="https://docs.microsoft.com/en-us/sharepoint/control-access-from-unmanaged-devices">의 sharepoint 및 OneDrive 콘텐츠 액세스를 차단 하거나 제한할</a> 수 있습니다.</span></p> <p><strong style="mso-bidi-font-weight: normal;"><u><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">네트워크 위치 제한</span></u></strong></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">IT 관리자는 사용자가 신뢰 하는 정의 된 네트워크 위치를 기반으로 SharePoint 및 OneDrive 리소스에 대 한 액세스를 제어할 수 있습니다. 이를 위치 기반 정책이 라고도 합니다. 자세한 내용은 <a href="https://docs.microsoft.com/en-us/sharepoint/control-access-based-on-network-location">네트워크 위치를 기반으로 SharePoint Online 및 OneDrive 데이터에 대 한 제어 액세스</a> 를 참조 하세요.</span></p> <p><strong style="mso-bidi-font-weight: normal;"><u><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">사이트 잠금 제한</span></u></strong></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">SharePoint Online 내에서는 사이트 모음을 잠글 수 있으므로 아무도 액세스 하지 못합니다. &nbsp; &ldquo; <em style="mso-bidi-font-style: normal;"><a href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps">Get-sposite</a></em> <em style="mso-bidi-font-style: normal;"> -</em> LockState&rdquo; 속성을 사용 하 여 PowerShell 및 <a href="https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps">SharePoint Online 관리 셸을</a> 통해이를 설정할 수 있습니다.</span></p> <p><strong style="mso-bidi-font-weight: normal;"><u><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">사용자가 사이트 또는 하위 사이트를 만들지 못하도록 제한</span></u></strong></p> <p><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">SharePoint 관리자 또는 Office 365 전역 관리자는 사용자가 자신의 SharePoint 사이트를 만들고 관리 하 고, 만들 수 있는 사이트 종류를 결정 하 고, 사이트의 위치를 지정 하도록 할 수 있습니다. 자세한 내용은 <a href="https://docs.microsoft.com/en-us/sharepoint/manage-site-creation">SharePoint Online에서 사이트 만들기 관리</a>를 참조 하세요.</span></p>
