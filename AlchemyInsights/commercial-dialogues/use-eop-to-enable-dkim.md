---
title: PowerShell을 Exchange Online 사용하여 특정 도메인에 대해 DKIM을 사용하도록 설정
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
ms.openlocfilehash: ba627c6da96624914b858aa09d6eff9de709134c2c986fe363845c5ab2b66434
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070312"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>PowerShell을 Exchange Online 사용하여 특정 도메인에 대해 DKIM을 사용하도록 설정

관리 센터에서 DKIM DNS 레코드를 만들 수 없는 경우 PowerShell을 사용하여 Exchange Online 합니다. 

PowerShell을 사용하여 DKIM DNS 레코드를 Exchange Online 다음 단계를 수행합니다.

1. 관리자 Windows PowerShell 열고 설명된 순서대로 다음 명령을 실행합니다.

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
PowerShell에 연결하는 데 Exchange Online 경우 PowerShell 커넥트 [Exchange Online 참조합니다.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. PowerShell에 Exchange Online 다음 명령을 실행합니다.

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. 위의 명령이 성공적으로 실행되면 다음 명령을 실행하여 PowerShell 세션을 Exchange Online 종료합니다.

    `Remove-PSSession $Session` 



