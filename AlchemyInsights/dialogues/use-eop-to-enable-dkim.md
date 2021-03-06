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
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a><span data-ttu-id="9d30a-102">Exchange Online PowerShell을 사용하여 특정 도메인에 대해 DKIM을 사용하도록 설정</span><span class="sxs-lookup"><span data-stu-id="9d30a-102">Use Exchange Online PowerShell to enable DKIM for a specific domain</span></span>

<span data-ttu-id="9d30a-103">관리 센터에서 DKIM DNS 레코드를 만들 수 없는 경우 Exchange Online PowerShell을 사용해 하세요.</span><span class="sxs-lookup"><span data-stu-id="9d30a-103">If you can't create the DKIM DNS records in the admin center, try using Exchange Online PowerShell.</span></span> 

<span data-ttu-id="9d30a-104">Exchange Online PowerShell을 사용하여 DKIM DNS 레코드를 만들 경우 다음 단계를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="9d30a-104">To create a DKIM DNS record using Exchange Online PowerShell, perform the following steps:</span></span>

1. <span data-ttu-id="9d30a-105">관리자 Windows PowerShell 열고 설명된 순서대로 다음 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="9d30a-105">Open Windows PowerShell as an administrator and run the following commands in the described sequence:</span></span>

    <span data-ttu-id="9d30a-106">a.</span><span class="sxs-lookup"><span data-stu-id="9d30a-106">a.</span></span> `$UserCredential = Get-Credential`

    <span data-ttu-id="9d30a-107">b.</span><span class="sxs-lookup"><span data-stu-id="9d30a-107">b.</span></span> `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="9d30a-108">c.</span><span class="sxs-lookup"><span data-stu-id="9d30a-108">c.</span></span> `Import-PSSession $Session -DisableNameChecking`
    
<span data-ttu-id="9d30a-109">Exchange Online PowerShell에 연결하는 데 문제가 있는 경우 [Exchange Online PowerShell에 연결을 참조하세요.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)</span><span class="sxs-lookup"><span data-stu-id="9d30a-109">If you have trouble connecting to Exchange Online PowerShell, see [Connect to Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="9d30a-110">Exchange Online PowerShell에 연결되면 다음 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="9d30a-110">Once you're connected to Exchange Online PowerShell, run the following command:</span></span>

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. <span data-ttu-id="9d30a-111">위의 명령이 성공적으로 실행되면 다음 명령을 실행하여 Exchange Online PowerShell 세션을 종료합니다.</span><span class="sxs-lookup"><span data-stu-id="9d30a-111">Once the above command has been successfully executed, run the following command to terminate the Exchange Online PowerShell session:</span></span>

    `Remove-PSSession $Session` 



