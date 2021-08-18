---
title: 탐색기에서 열기를 사용하여 문제 해결
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
ms.openlocfilehash: 49d6d449af6e718d70c9948a03f7e2e1e21517d2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323572"
---
# <a name="fix-problems-with-open-with-explorer"></a>탐색기에서 열기 문제 해결

탐색기에서 열기 명령을 사용하여 SharePoint OneDrive **라이브러리를 여는** 경우의 일반적인 문제를 해결합니다. 
  
- 11 Internet Explorer 10 Internet Explorer 사용 **탐색기에서 열기는** Microsoft Edge, Google Chrome, Firefox 등과 호환되지 않습니다. **탐색기를 사용하여** 열기는 탐색기를 제외한 모든 브라우저에서 Internet Explorer. 
    
- **탐색기를 사용하여 열기는** 사용자 라이브러리의 최신 SharePoint 없습니다. 대신 **파일 탐색기에서 보기를** 사용합니다. 파일 **탐색기에서** \> **보기 옵션 보기를 선택합니다.** 파일 탐색기에서 보기는 Microsoft Edge, Google Chrome, Firefox 등과 호환되지 않습니다. **파일 탐색기에서 보기를** 사용할 수 있는 Internet Explorer. 
    
- WebClient 서비스가 실행되고 있는지 확인 앱 Windows 입력하고, 데스크톱 앱 실행을 선택하고, services.msc를 입력한 다음 Enter를 누를 수 있습니다. 아래로 스크롤하여 WebClient 서비스로  이동한 다음 상태 열에 "실행 중"이 표시되고 있는지 확인할 수 있습니다. 그렇지 않은 경우 서비스를 두 번 클릭하고 **시작을** 클릭한 다음 확인 을 **클릭합니다.** 시작 유형 상자에서 수동 또는 자동을  선택하여  서비스를 사용하도록 **설정해야** 할 수 있습니다. 
    
**참고:** 여러 파일 및 폴더를 한 번 복사하거나 이동해야 하는 경우 파일 탐색기에서 라이브러리를 열면 도움이 되지만 라이브러리에서 정기적으로 작업하려는 경우 라이브러리를 동기화하는 것이 좋습니다. 파일 탐색기에서 열기 문제를 해결하려면 [탐색기에서 열기를 참조합니다.](https://go.microsoft.com/fwlink/?linkid=871665) 동기화 설정에 대한 자세한 내용은 새 SharePoint 클라이언트와 파일 [동기화를 OneDrive 동기화 참조하세요.](https://go.microsoft.com/fwlink/?linkid=871666)
  
자세한 내용은 [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) 문서를 참조하세요. 
  

