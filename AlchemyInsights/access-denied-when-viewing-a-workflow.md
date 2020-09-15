---
title: 워크플로를 볼 때 액세스 거부 됨
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688808"
---
# <a name="access-denied-when-viewing-a-workflow"></a>워크플로를 볼 때 액세스 거부 됨

Sharepoint 2013 sharepoint 그룹의 구성원 자격이 모든 사람으로 설정 되어 있지 않으면 SharePoint 그룹에 전자 메일을 보내려고 할 때 "액세스 거부" 라는 오류 메시지가 나타나지 않을 수 있습니다.
  
 **이 문제를 해결 하려면 다음 단계를 수행 합니다.**
  
 1. 모든 사람이 SharePoint 그룹의 구성원을 볼 수 있도록 허용 합니다.
  
 2. 전자 메일의 받는 사람 또는 참조 줄에서 SharePoint 그룹을 제거 합니다.
  
 3. SharePoint 그룹에 대 한 멤버 자격 표시 유형을 변경할 수 없는 경우 To 또는 CC 줄에 사용자를 명시적으로 추가 합니다.
  
자세한 내용을 보려면 [HTTP가 허용 되지 않음/_vti_bin/client.svc/sp.utilities.utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)를 참조 하세요.
  