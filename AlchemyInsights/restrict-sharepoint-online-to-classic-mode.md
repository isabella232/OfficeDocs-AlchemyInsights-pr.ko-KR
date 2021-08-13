---
title: 온라인 SharePoint 모드로 제한
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
ms.openlocfilehash: 6315a83ac825f96ceea60798d441de8e8e53336fe29eda4d0491dd8a6a43b352
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53958807"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>온라인 SharePoint 모드로 제한

일부 조직에서는 여전히 클래식 모드 환경이 필요한 경우도 있습니다. 세부적인 수준에서 클래식 모드를 제거할 계획이 없는 경우 목록 및 라이브러리의 클래식 모드로 전체 조직(테넌트)을 제한할 수 없습니다.

관리자는 다음 수준에서 제공하는 세분된 옵트아웃 스위치를 사용하여 클래식 모드에서 개별 목록 및 라이브러리를 관리할 수 있는 다음 옵션을 사용할 수 있습니다.

- 사이트 모음
- site
- list
- library

또한 최신에서 지원되지 않는 특정 기능 및 사용자 지정을 사용하는 목록은 여전히 클래식 모드로 자동 전환됩니다.

2019년 4월 1일부터 테넌트 수준이 최신 목록에서 옵트아웃(opt out)을 사용하지 않도록 설정하는 프로세스가 시작되고 2019년 5월 31일까지 계속됩니다.  테넌트 옵트아웃의 결과로 클래식 모드에 있는 목록 및 라이브러리는 자동으로 최신 모드로 전환됩니다.

클래식 모드가 필요한 경우 [](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) 여기에서 클래식 모드 환경을 사용하는 [](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) 데 사용할 수 있는 옵션 및 도구를 설명하는 PnP Powershell 명령을 참조하세요.
