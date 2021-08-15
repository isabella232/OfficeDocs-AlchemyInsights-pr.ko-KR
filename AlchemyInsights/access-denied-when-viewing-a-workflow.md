---
title: 워크플로를 볼 때 액세스 거부
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 2b076ec5dca070555ce51b88631fb6bd619ed9269e59ccc799b23b8b95547c16
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955207"
---
# <a name="access-denied-when-viewing-a-workflow"></a>워크플로를 볼 때 액세스 거부

SharePoint 2013 SharePoint 그룹의 구성원이 모든 사용자로 설정되지 않은 경우 "액세스 거부 SharePoint" 오류 메시지가 표시될 수 있습니다.
  
 **이 문제를 해결하기 위해 다음 단계를 수행합니다.**
  
 1. 모든 사용자가 그룹 구성원을 볼 SharePoint 허용합니다.
  
 2. 전자 메일의 SharePoint 또는 CC 줄에서 메일 그룹을 제거합니다.
  
 3. 그룹 구성원 자격 표시를 변경할 수 없는 경우 사용자를 To 또는 CC 줄에 명시적으로 SharePoint 있습니다.
  
자세한 내용을 보려면 HTTP 권한이 없는 [경우 /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)을 참조하시기 바랍니다.
  