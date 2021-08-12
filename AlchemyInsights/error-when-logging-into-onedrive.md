---
title: 0x8004de40 때 오류가 OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: 23c57356c8bd94c1cbafb538c9318208429754115a7c4e88abc93d293b5ea6e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946585"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 때 오류가 OneDrive

로그인할 **때** 0x8004de40 오류가 OneDrive 또는 학교 도메인에 연결된 동안 컴퓨터를 다시 시작하십시오. 다시 부팅한 후 이 오류가 표시되면 직장 또는 학교 도메인에 연결된 동안 시도해 보아야 합니다.

1. 시작을 클릭하고 검색  상자에 **cmd** 또는 명령 프롬프트를 입력하고 명령 프롬프트 앱을 마우스 오른쪽 단추로 클릭한 다음 **관리자 권한으로 실행을 선택합니다.** 관리자 암호를 입력하거나 확인 메시지를 표시하는 경우 암호를 입력하거나 허용 을 **클릭합니다.**  

2. 명령 프롬프트 창에 **dsregcmd /leave를**  입력하고 명령이 완료될 때까지 기다립니다. 그런 다음 **dsregcmd /join을 입력하고** 명령이 완료될 때까지 기다릴 수 있습니다.
3. 컴퓨터를 다시 시작하십시오.
