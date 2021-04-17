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
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819518"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="ffd27-102">Outlook에서 공용 폴더에 연결할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="ffd27-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="ffd27-103">일부 사용자에 대해 공용 폴더 액세스가 작동하지 않는 경우 다음을 시도합니다.</span><span class="sxs-lookup"><span data-stu-id="ffd27-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="ffd27-104">EXO PowerShell에 연결하고 문제 사용자 계정의 DefaultPublicFolderMailbox 매개 변수를 작업 사용자 계정의 매개 변수와 일치하도록 구성합니다.</span><span class="sxs-lookup"><span data-stu-id="ffd27-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="ffd27-105">예제:</span><span class="sxs-lookup"><span data-stu-id="ffd27-105">Example:</span></span>

<span data-ttu-id="ffd27-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="ffd27-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="ffd27-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="ffd27-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="ffd27-108">변경이 적용될 때까지 1시간 이상 기다릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ffd27-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="ffd27-109">문제가 계속 발생하면 다음 절차에 [따라](https://aka.ms/pfcte) Outlook을 사용하여 공용 폴더 액세스 문제를 해결하십시오.</span><span class="sxs-lookup"><span data-stu-id="ffd27-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="ffd27-110">Outlook을 사용하여 공용 폴더에 액세스할 수 **있는 사용자를 제어합니다.**</span><span class="sxs-lookup"><span data-stu-id="ffd27-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="ffd27-111">-Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true $false</span><span class="sxs-lookup"><span data-stu-id="ffd27-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="ffd27-112">$true: Outlook의 공용 폴더에 대한 사용자 액세스 허용</span><span class="sxs-lookup"><span data-stu-id="ffd27-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="ffd27-113">$false: Outlook의 공용 폴더에 대한 사용자 액세스 차단</span><span class="sxs-lookup"><span data-stu-id="ffd27-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="ffd27-114">이 값은 기본값입니다.</span><span class="sxs-lookup"><span data-stu-id="ffd27-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="ffd27-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="ffd27-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="ffd27-116">**참고** 이 절차에서는 Windows 클라이언트용 Outlook 데스크톱에서만 연결을 제어할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ffd27-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="ffd27-117">사용자는 OWA 또는 Mac용 Outlook을 사용하여 공용 폴더에 계속 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ffd27-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="ffd27-118">자세한 내용은 Outlook의 공용 폴더에 대한 제어된 연결 지원 [발표를 참조하세요.](https://aka.ms/controlpf)</span><span class="sxs-lookup"><span data-stu-id="ffd27-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>