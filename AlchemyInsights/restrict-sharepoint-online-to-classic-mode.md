---
title: SharePoint Online을 클래식 모드로 제한
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751428"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>SharePoint Online을 클래식 모드로 제한

일부 조직은 여전히 클래식 모드 환경을 필요로 합니다. 클래식 모드를 세분화 된 수준에서 제거할 계획이 없는 경우에는 더 이상 목록 및 라이브러리에 대 한 전체 조직 (테 넌 트)을 클래식 모드로 제한할 수 없습니다.

관리자는 다음과 같은 수준에서 제공 하는 세분화 된 옵트아웃 스위치를 사용 하 여 클래식 모드에서 개별 목록 및 라이브러리를 관리할 수 있는 다음과 같은 옵션을 사용할 수 있습니다.

- 사이트 모음
- 사이트
- 목록
- 라이브러리

또한 현대에서 지원 되지 않는 특정 기능 및 사용자 지정 내용을 사용 하는 목록은 여전히 클래식 모드로 자동 전환 됩니다.

2019 년 4 월 1 일부 터, 최신 목록 및 라이브러리에 대 한 테 넌 트 수준 옵트아웃을 사용 하지 않도록 설정 하는 프로세스는 시작 하 고 5 월 31 2019 일까지 계속 진행 됩니다.  테 넌 트 옵트아웃의 결과로 클래식 모드에 있는 목록 및 라이브러리는 자동으로 최신으로 이동 됩니다.

클래식 모드를 사용 해야 하는 경우 여기 및 PnP Powershell 명령 [여기](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) 에는 클래식 모드 환경을 사용할 때 사용할 수 있는 옵션 및 도구에 [대 한 추가 정보를](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) 참조 하세요.
