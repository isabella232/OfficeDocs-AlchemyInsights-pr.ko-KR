---
title: 탐색기에서 열기가 작동하지 않습니다.
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
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 164d5fe8c992df825d1f52f19792e1623526c35c58ff2f1e1ab601fdcf5f0f53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011342"
---
# <a name="open-with-explorer-isnt-working"></a>탐색기가 작동하지 않는 경우 열기

파일 **탐색기에서 열기** 또는 파일 탐색기에서 보기가 작동하지 않는  경우 아래 단계에 따라 WebClient 서비스가 실행 중으로 설정되어 있는지 확인하십시오.  예를 들어 서비스가 실행되고 있지 않은 경우 SharePoint OneDrive 라이브러리를 여는 데 시간이 오래 걸릴 수 있습니다. 
  
1. 검색 Windows 입력하고 실행 데스크톱 앱을 선택하고 services.msc를 입력한 다음 Enter 를 **선택합니다.**
    
2. 아래로 스크롤하여 WebClient 서비스로 이동한 다음 상태 **열을** 검사합니다. WebClient 서비스 상태가 실행되고 있지 않은 경우 서비스를 두 번 클릭하고 **시작을** 클릭한 다음 확인을 **클릭합니다.**  필요한 경우 시작 유형 상자에서 **수동** 또는  자동을 선택하여 서비스를 **사용하도록** 설정하십시오. 
    
> [!NOTE]
> 파일 탐색기에서 열기 문제를 해결하려면 [탐색기에서 열기를 참조합니다.](https://go.microsoft.com/fwlink/?linkid=871665) 더 나은 대안으로 동기화를 탐색합니다. SharePoint 클라이언트와 동기화를 OneDrive 동기화 [합니다.](https://go.microsoft.com/fwlink/?linkid=871666) 
  

