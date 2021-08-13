---
title: Active Directory가 동기화되지 않습니다.
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
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 4bfbe6b2dd9a2112f0cb7af0d6e7a46693bc70680895fd674ddb0332b7071797
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53937107"
---
# <a name="active-directory-not-syncing"></a>Active Directory가 동기화되지 않습니다.

"최근 동기화 없음"처럼 동기화 오류가 수신되거나 Office 관리 포털의 디렉터리 동기화 상태가 "마지막으로 동기화된 지 3일이 지난"이면 AADConnect에 동기화를 수행할 수 있는 권한이 잘못되거나 권한이 부족한 것일 수 있습니다.  

익스프레스 설정을 사용하여 AADConnect를 다시하면 문제가 빠르게 해결될 수 있습니다.

1. [최신 버전의 AADConnect를 다운로드합니다.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [익스프레스 설치에 대한 지침을 따릅니다.](/azure/active-directory/hybrid/how-to-connect-install-express)

Azure AD Connect는 Windows Server 2012 이상에 설치해야 합니다. 이 서버는 도메인에 연결되어 있어야 하며 도메인 컨트롤러나 구성원 서버일 수 있습니다. Azure AD 요구 사항 및 커넥트 전체 목록은 [Azure AD](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)커넥트.

AADConnect 서비스 계정에 대한 자세한 내용은 [Azure AD Connect:계정 및 사용 권한](/azure/active-directory/hybrid/reference-connect-accounts-permissions)을 참조하세요.
