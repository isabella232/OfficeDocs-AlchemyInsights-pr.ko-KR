---
title: OneDrive에서 0x8004de40 오류 수정
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745136"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>OneDrive에서 0x8004de40 오류 수정

OneDrive와 함께 0x8004de40 오류가 표시 되는 경우:

- Acitve 디렉터리 도메인에 연결 된 상태에서 영향을 받는 컴퓨터를 다시 부팅 합니다.
- 다시 부팅 해도 문제가 해결 되지 않으면 Azure AD에서 디바이스를 가입 하지 않고 참가 시킵니다. 

**참고**: 다음 단계를 수행 하는 동안 회사 네트워크에 있어야 합니다. 회사 인프라 (예: 여행 중)에 연결할 수 없는 경우에는이 단계를 수행 하지 마십시오. 

- 승격된 명령 프롬프트를 엽니다. 
- 관리자 권한 명령 프롬프트를 열려면- **Start**를 클릭 하 고 **명령 프롬프트**를 마우스 오른쪽 단추로 클릭 한 다음 **관리자 권한으로 실행**을 클릭 합니다.
- *Dsregcmd/leave* 를 입력 하 고 enter 키 **를 누릅니다.**
- 완료 되 면 *dsregcmd/join* 을 입력 하 **고 enter 키를 누릅니다.**
- 완료 되 면 명령 프롬프트를 닫습니다.
- 컴퓨터를 다시 부팅 하 고 OneDrive에 로그인 합니다.