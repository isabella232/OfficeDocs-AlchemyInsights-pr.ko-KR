---
title: ClientAccessServerEnabled를 True로 설정
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50510004"
---
# <a name="set-clientaccessserverenabled-to-true"></a>ClientAccessServerEnabled를 True로 설정

암호화된 전자 메일 메시지를 열 수 없는 대신 **rpmsg** 첨부 파일이 표시되어 있는 경우 다음 단계를 수행합니다.

1. Exchange Online PowerShell에 연결합니다.

> [!NOTE]
> Exchange Online PowerShell에 연결하려면 전역 관리자 또는 Exchange 관리자 계정을 사용하여 로그인해야 합니다.

   a. 다음 Windows PowerShell 열고 다음 명령을 실행합니다. `$UserCredential = Get-Credential`
b. 자격 **증명 Windows PowerShell** 대화 상자에 직장 또는 학교 계정과 암호를 입력합니다. c. **확인** 을 클릭합니다. 

2. 다음 명령을 실행하여 새 세션을 만들 수 있습니다.

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. 다음 명령을 실행합니다.
    
    `Import-PSSession $Session -DisableNameChecking`

3. 명령을 `Get-IRMConfiguration` 실행합니다.

4. **ClientAccessServerEnabled 설정을** 검사합니다. 

    a. **ClientAccessServerEnabled** 설정이 **False로** 설정된 경우 다음 cmdlet을 실행합니다.`Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> 항상 다음 명령을 사용하여 powershell 세션을 닫습니다. `Remove-PSSession $Session`

자세한 내용은 [Exchange Online PowerShell 을 참조하세요.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

