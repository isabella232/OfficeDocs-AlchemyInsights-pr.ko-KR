---
title: 암호 동기화 문제 해결
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387883"
---
# <a name="troubleshoot-password-synchronization"></a>암호 동기화 문제 해결

암호 동기화 문제를 해결 하려면이 AAD 연결 문제 해결 작업을 사용 하 여 암호가 동기화 되지 않는 이유를 확인 합니다. 시작 하려면 [직접 동기화 관리](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)로 이동 합니다.  

1. Azure AD Connect 서버에서 새 Windows PowerShell 세션을 열고 **관리자 권한으로 실행** 옵션을 선택 합니다.

2. ExecutionPolicy RemoteSigned 또는 ExecutionPolicy 제한이 없는 경우 실행 합니다.

3. Azure AD Connect 마법사를 시작 합니다.

4. 다음에 대 한 **문제 해결**> 추가 작업 페이지로 이동  >  **Next**합니다.

5. **시작** 을 선택 하 여 PowerShell 문제 해결 메뉴를 엽니다.

6. **암호 동기화 문제 해결**을 선택 합니다.

    이 문제는 일반적으로 특정 사용자 계정에 대해 암호가 동기화 되지 않은 경우에 발생 합니다.

    **참고 사항** 마지막으로 성공한 암호 동기화가 잠시 전에 암호 동기화가 실패 합니다.

암호 동기화 문제 해결에 대 한 자세한 내용은 [AZURE AD Connect sync를 통한 암호 해시 동기화 문제 해결](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)을 참조 하세요.