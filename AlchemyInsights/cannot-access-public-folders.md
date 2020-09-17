---
title: 공용 폴더에 액세스할 수 없음
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
- "3500007"
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812553"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook에서 공용 폴더에 연결할 수 없음

일부 사용자가 공용 폴더 액세스가 작동 하지 않는 경우 다음을 시도해 보세요.

EXO PowerShell에 연결 하 고 문제 사용자 계정에 대해 DefaultPublicFolderMailbox 매개 변수를 구성 하 여 작업 중인 사용자 계정의 매개 변수와 일치 시킵니다.

예제:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

ProblemUser-DefaultPublicFolderMailbox \<value from previous command>

변경 내용이 적용 되려면 한 시간 이상 기다립니다.

문제가 계속 되 면 다음 [절차](https://aka.ms/pfcte) 에 따라 Outlook을 사용 하 여 공용 폴더 액세스 문제를 해결 하세요.
 
**Outlook을 사용 하 여 공용 폴더에 액세스할 수 있는 사용자를 제어 하려면**:

1.  설정-CASMailbox <mailboxname> -publicfolderclientaccess $true 또는 $false를 사용 합니다.  
      
    $true: Outlook의 공용 폴더에 대한 사용자 액세스 허용  
      
    $false: Outlook의 공용 폴더에 대한 사용자 액세스 차단 이 값은 기본값입니다.  
        
2.  Set-organizationconfig-PublicFolderShowClientControl $true   
      
**참고 사항** 이 절차는 Windows 클라이언트용 Outlook desktop을 사용 하 여 연결만 제어할 수 있습니다. 사용자는 OWA 또는 Mac 용 Outlook을 사용 하 여 공용 폴더에 계속 액세스할 수 있습니다.
 
자세한 내용은 [Outlook에서 공용 폴더에 대 한 제어 되는 연결 지원 발표](https://aka.ms/controlpf)를 참조 하십시오.