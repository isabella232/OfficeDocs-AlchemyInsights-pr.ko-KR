---
title: 암호 동기화 문제 해결
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: cb782c0d1dc396ee7a9f016afb9629a2cdee93d52f5408b7a73e576e783ebc0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105760"
---
# <a name="troubleshoot-password-synchronization"></a>암호 동기화 문제 해결

암호 동기화 문제를 해결하기 위해 먼저 이 AAD 커넥트 문제 해결 작업을 사용하여 암호가 동기화되지 않는 이유를 파악합니다. 먼저 직접 동기화 [관리로 이동 합니다.](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)  

1. Azure AD Windows PowerShell 서버에서 새 커넥트 세션을 열고 관리자 권한으로 실행 **옵션을** 선택합니다.

2. RemoteSigned Set-ExecutionPolicy 무제한으로 Set-ExecutionPolicy 실행합니다.

3. Azure AD 서비스 커넥트 시작하세요.

4. 추가 작업 페이지로 이동하여 > **다음 문제 해결**  >  **으로 이동합니다.**

5. 실행을 **선택하여** PowerShell 문제 해결 메뉴를 열 수 있습니다.

6. 암호 **동기화 문제 해결 을 선택합니다.**

    문제는 일반적으로 특정 사용자 계정에 대해 암호가 동기화되지 않는 것입니다.

    **참고** 마지막으로 성공한 암호 동기화가 몇 시간 전이면 암호 동기화가 실패합니다.

암호 동기화 문제를 해결하는 데 도움이 되는 자세한 내용은 Azure AD 동기화를 사용하여 암호 해시 [커넥트 참조하세요.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)