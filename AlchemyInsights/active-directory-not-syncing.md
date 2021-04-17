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
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822857"
---
# <a name="active-directory-not-syncing"></a>Active Directory가 동기화되지 않습니다.

"최근 동기화 없음"처럼 동기화 오류가 수신되거나 Office 관리 포털의 디렉터리 동기화 상태가 "마지막으로 동기화된 지 3일이 지난"이면 AADConnect에 동기화를 수행할 수 있는 잘못된 설정이나 권한이 부족한 것일 수 있습니다.  

익스프레스 설정을 사용하여 AADConnect를 다시설치하면 문제가 빠르게 해결될 수 있습니다.

1. [최신 버전의 AADConnect를 다운로드합니다.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [익스프레스 설치에 대한 지침을 따릅니다.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)

AADConnect 서비스 계정에 대한 자세한 내용은 [Azure AD Connect:계정 및 사용 권한](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)을 참조하세요.
