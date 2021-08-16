---
title: 공용 폴더에 액세스할 수 없습니다.
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
- "3500007"
- "3462"
ms.openlocfilehash: f129da8731877aa00fd9b1dcf20905d353a4895303390ce7ff5642a8ff3ccbc2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53996636"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook 폴더에 연결할 수 없습니다.

일부 사용자에 대해 공용 폴더 액세스가 작동하지 않는 경우 다음을 시도합니다.

커넥트 작업 사용자 계정의 매개 변수와 일치하도록 EXO PowerShell에 연결하고 문제 사용자 계정에 DefaultPublicFolderMailbox 매개 변수를 구성합니다.

예:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

변경이 적용될 때까지 1시간 이상 기다릴 수 있습니다.

문제가 계속되는 경우 [](https://aka.ms/pfcte) 다음 절차에 따라 공용 폴더 액세스 문제를 Outlook.
 
**다음을 사용하여** 공용 폴더에 액세스할 수 있는 사용자를 Outlook.

1.  -Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true $false  
      
    $true: Outlook의 공용 폴더에 대한 사용자 액세스 허용  
      
    $false: Outlook의 공용 폴더에 대한 사용자 액세스 차단 이 값은 기본값입니다.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**참고** 이 절차에서는 클라이언트의 데스크톱에서만 Outlook 수 Windows 있습니다. 사용자는 OWA 또는 Mac용 폴더를 사용하여 공용 폴더에 Outlook 수 있습니다.
 
자세한 내용은 에서 공용 폴더에 대한 제어된 연결 지원 [발표를 Outlook.](https://aka.ms/controlpf)