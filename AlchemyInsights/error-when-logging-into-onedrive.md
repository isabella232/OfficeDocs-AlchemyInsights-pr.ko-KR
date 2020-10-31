---
title: OneDrive를 시작할 때 발생 하는 오류 0x8004de40
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/30/2020
ms.locfileid: "48815994"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>OneDrive를 시작할 때 발생 하는 오류 0x8004de40

OneDrive에 로그인 할 때 오류 **0x8004de40** 이 나타나면 회사 또는 학교 도메인에 연결 된 상태에서 컴퓨터를 다시 부팅 합니다. 다시 부팅 한 후에이 오류가 나타나면 회사 또는 학교 도메인에 연결 되어 있는 동안 다음을 수행 합니다.

1. 시작을 클릭 하 고 검색 상자에 **cmd** 또는 **명령 프롬프트**  를 입력 하 고 명령 프롬프트 앱을 마우스 오른쪽 단추로 클릭 한 다음  **관리자 권한으로 실행** 을 선택 합니다. 관리자 암호나 확인을 묻는 메시지가 표시 되 면 암호를 입력 하거나 **허용** 을 클릭 합니다.  

2. 명령 프롬프트 창에서 **dsregcmd/leave**  를 입력 하 고 명령이 완료 될 때까지 기다립니다. 그런 다음 **dsregcmd/tjoin** 을 입력 하 고 명령이 완료 될 때까지 기다립니다.
3. 컴퓨터를 다시 부팅 합니다.
