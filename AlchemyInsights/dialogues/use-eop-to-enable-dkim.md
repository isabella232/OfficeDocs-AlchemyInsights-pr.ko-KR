---
title: Exchange Online PowerShell을 사용하여 특정 도메인에 대해 DKIM을 사용하도록 설정
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50500882"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Exchange Online PowerShell을 사용하여 특정 도메인에 대해 DKIM을 사용하도록 설정

관리 센터에서 DKIM DNS 레코드를 만들 수 없는 경우 Exchange Online PowerShell을 사용해 하세요. 

Exchange Online PowerShell을 사용하여 DKIM DNS 레코드를 만들 경우 다음 단계를 수행합니다.

1. 관리자 Windows PowerShell 열고 설명된 순서대로 다음 명령을 실행합니다.

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Exchange Online PowerShell에 연결하는 데 문제가 있는 경우 [Exchange Online PowerShell에 연결을 참조하세요.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. Exchange Online PowerShell에 연결되면 다음 명령을 실행합니다.

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. 위의 명령이 성공적으로 실행되면 다음 명령을 실행하여 Exchange Online PowerShell 세션을 종료합니다.

    `Remove-PSSession $Session` 



