---
title: SharePoint Designer 연결 문제
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
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727177"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer 연결 문제 

SharePoint Designer에 SharePoint 사이트에 대 한 연결 문제가 발생 하는 경우 다음과 같은 일반적인 해결 방법을 시도해 보세요.

1 단계: sharepoint designer 2013이 sharepoint designer [서비스 팩 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) 과 [8 월 2 일, 2016 Update for sharepoint designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)에 업데이트 되어 있는지 확인 합니다.



2 단계: 로컬 캐시 파일 지우기:

1. SharePoint Designer 2013을 닫습니다.

2. 로컬 컴퓨터에서 다음 폴더 각각에 있는 파일을 모두 제거 합니다.

    - %APPDATA%\Microsoft\Web 서버 Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. SharePoint Designer 2013를 열고 계정을 다시 입력 하 여 작동 하는지 확인 합니다.

3 단계: [Windows 장치에서 Office 2013에 대 한 최신 인증을 사용 하도록 설정](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)합니다.

4 단계: 관리자는 sharepoint 관리 센터 설정에서 **사용자 지정 스크립트를 허용** 하 여이 연결을 허용 해야 합니다. 자세한 내용은 [사용자 지정 스크립트 허용 또는 금지](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) 를 참조 하세요.


