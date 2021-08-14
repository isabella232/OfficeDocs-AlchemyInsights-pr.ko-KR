---
title: SharePoint 디자이너 연결 문제
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: d55f7c1902bb623900fa74bdae70695b6e04ad84ce7b6ea314db614283ec436d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53942031"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint 디자이너 연결 문제 

SharePoint 사이트와의 연결 SharePoint 발생하는 경우 다음과 같은 일반적인 해결 방법을 시도해 보아야 합니다.

1단계: SharePoint Designer 2013이 SharePoint [Designer](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) 2013용 [2016년 8월 2일 업데이트 및 SharePoint Designer 2013으로 업데이트되어](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)있는지 확인



2단계: 로컬 캐시 파일 지우기:

1. SharePoint Designer 2013을 닫습니다.

2. 로컬 컴퓨터에서 다음 폴더에 있는 모든 파일을 제거합니다.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. SharePoint Designer 2013을 열고 계정을 다시 입력하여 작동하는지 볼 수 있습니다.

3단계: 모바일 장치에서 Office [2013에](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)대해 최신 Windows 사용하도록 설정

4단계: 관리자는 SharePoint  Designer 연결을 허용하려면 SharePoint 사용자 지정 스크립트를 허용해야 SharePoint 합니다. 자세한 [내용은 사용자 지정 스크립트 허용 또는](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) 금지를 참조하세요.


