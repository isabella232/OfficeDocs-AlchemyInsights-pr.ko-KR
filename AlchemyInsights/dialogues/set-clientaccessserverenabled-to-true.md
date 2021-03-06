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
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="8d040-102">ClientAccessServerEnabled를 True로 설정</span><span class="sxs-lookup"><span data-stu-id="8d040-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="8d040-103">암호화된 전자 메일 메시지를 열 수 없는 대신 **rpmsg** 첨부 파일이 표시되어 있는 경우 다음 단계를 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="8d040-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="8d040-104">Exchange Online PowerShell에 연결합니다.</span><span class="sxs-lookup"><span data-stu-id="8d040-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="8d040-105">Exchange Online PowerShell에 연결하려면 전역 관리자 또는 Exchange 관리자 계정을 사용하여 로그인해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="8d040-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="8d040-106">a.</span><span class="sxs-lookup"><span data-stu-id="8d040-106">a.</span></span> <span data-ttu-id="8d040-107">다음 Windows PowerShell 열고 다음 명령을 실행합니다. `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="8d040-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="8d040-108">b.</span><span class="sxs-lookup"><span data-stu-id="8d040-108">b.</span></span> <span data-ttu-id="8d040-109">자격 **증명 Windows PowerShell** 대화 상자에 직장 또는 학교 계정과 암호를 입력합니다. c.</span><span class="sxs-lookup"><span data-stu-id="8d040-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="8d040-110">**확인** 을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="8d040-110">Click **OK**.</span></span> 

2. <span data-ttu-id="8d040-111">다음 명령을 실행하여 새 세션을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8d040-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="8d040-112">a.</span><span class="sxs-lookup"><span data-stu-id="8d040-112">a.</span></span> <span data-ttu-id="8d040-113">다음 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="8d040-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="8d040-114">명령을 `Get-IRMConfiguration` 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="8d040-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="8d040-115">**ClientAccessServerEnabled 설정을** 검사합니다.</span><span class="sxs-lookup"><span data-stu-id="8d040-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="8d040-116">a.</span><span class="sxs-lookup"><span data-stu-id="8d040-116">a.</span></span> <span data-ttu-id="8d040-117">**ClientAccessServerEnabled** 설정이 **False로** 설정된 경우 다음 cmdlet을 실행합니다.`Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="8d040-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="8d040-118">항상 다음 명령을 사용하여 powershell 세션을 닫습니다. `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="8d040-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="8d040-119">자세한 내용은 [Exchange Online PowerShell 을 참조하세요.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)</span><span class="sxs-lookup"><span data-stu-id="8d040-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

