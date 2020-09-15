---
title: 탐색기에서 열기를 사용 하 여 문제 해결
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659064"
---
# <a name="fix-problems-with-open-with-explorer"></a>탐색기에서 열기 문제 해결

**탐색기에서 열기** 명령을 사용 하 여 SharePoint 또는 OneDrive에서 문서 라이브러리를 여는 일반적인 문제를 해결 합니다. 
  
- Internet Explorer 10 또는 Internet Explorer 11을 사용 합니다. **탐색기에서 열기** 는 Microsoft Edge, Google Chrome, Firefox 및 기타 기능과 호환 되지 않습니다. Internet Explorer를 제외한 모든 브라우저에서는 **탐색기에서 열기** 를 사용할 수 없습니다. 
    
- 현재 SharePoint 라이브러리 환경에서는 **탐색기에서 열기** 를 사용할 수 없습니다. 대신 **파일 탐색기에서 보기를** 사용 합니다. **View options** \> **파일 탐색기에서 보기 옵션 보기를**선택 합니다. 파일 탐색기의 보기는 Microsoft Edge, Google Chrome, Firefox 및 기타와 호환 되지 않습니다. Internet Explorer 에서만 사용할 수 있는 **파일 탐색기의 보기** 입니다. 
    
- WebClient 서비스가 실행 되 고 있는지 확인 합니다. Windows 검색 상자에 실행을 입력 하 고 데스크톱 실행 앱을 선택 하 고 services.msc를 입력 한 다음 enter 키를 누릅니다. 아래로 스크롤하여 WebClient 서비스를 확인 하 고 **상태** 열에 "실행 중"이 표시 되도록 합니다. 그렇지 않으면 서비스를 두 번 클릭 하 고 **시작**을 클릭 한 다음 **확인**을 클릭 합니다. ( **시작 유형** 상자에서 **수동** 또는 **자동** 을 선택 하 여 서비스를 먼저 사용 하도록 설정 해야 할 수 있습니다.) 
    
> [!NOTE]
> 파일 탐색기에서 라이브러리를 여는 것은 여러 파일 및 폴더를 한 번 복사 하거나 이동 해야 하지만 라이브러리에서 정기적으로 작업 하려는 경우 동기화 하는 것이 좋습니다. 파일 탐색기에서 열기 문제를 해결 하려면 [탐색기에서 열기](https://go.microsoft.com/fwlink/?linkid=871665)를 참조 하십시오. 동기화 설정에 대 한 자세한 내용은 [SharePoint 파일을 새 OneDrive 동기화 클라이언트와 동기화](https://go.microsoft.com/fwlink/?linkid=871666)를 참조 하세요.
  
자세한 내용은 [SharePoint Online의 문제를 해결 하기 위해 "탐색기에서 열기" 명령을 사용](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) 하는 방법에 대 한 문서를 참조 하세요. 
  

