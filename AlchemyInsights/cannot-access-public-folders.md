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
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="6cedc-102">Outlook에서 공용 폴더에 연결할 수 없음</span><span class="sxs-lookup"><span data-stu-id="6cedc-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="6cedc-103">일부 사용자가 공용 폴더 액세스가 작동 하지 않는 경우 다음을 시도해 보세요.</span><span class="sxs-lookup"><span data-stu-id="6cedc-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="6cedc-104">EXO PowerShell에 연결 하 고 문제 사용자 계정에 대해 DefaultPublicFolderMailbox 매개 변수를 구성 하 여 작업 중인 사용자 계정의 매개 변수와 일치 시킵니다.</span><span class="sxs-lookup"><span data-stu-id="6cedc-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="6cedc-105">예제:</span><span class="sxs-lookup"><span data-stu-id="6cedc-105">Example:</span></span>

<span data-ttu-id="6cedc-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="6cedc-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="6cedc-107">ProblemUser-DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="6cedc-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="6cedc-108">변경 내용이 적용 되려면 한 시간 이상 기다립니다.</span><span class="sxs-lookup"><span data-stu-id="6cedc-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="6cedc-109">문제가 계속 되 면 다음 [절차](https://aka.ms/pfcte) 에 따라 Outlook을 사용 하 여 공용 폴더 액세스 문제를 해결 하세요.</span><span class="sxs-lookup"><span data-stu-id="6cedc-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="6cedc-110">**Outlook을 사용 하 여 공용 폴더에 액세스할 수 있는 사용자를 제어 하려면**:</span><span class="sxs-lookup"><span data-stu-id="6cedc-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="6cedc-111">설정-CASMailbox <mailboxname> -publicfolderclientaccess $true 또는 $false를 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="6cedc-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="6cedc-112">$true: Outlook의 공용 폴더에 대한 사용자 액세스 허용</span><span class="sxs-lookup"><span data-stu-id="6cedc-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="6cedc-113">$false: Outlook의 공용 폴더에 대한 사용자 액세스 차단</span><span class="sxs-lookup"><span data-stu-id="6cedc-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="6cedc-114">이 값은 기본값입니다.</span><span class="sxs-lookup"><span data-stu-id="6cedc-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="6cedc-115">Set-organizationconfig-PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="6cedc-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="6cedc-116">**참고 사항** 이 절차는 Windows 클라이언트용 Outlook desktop을 사용 하 여 연결만 제어할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6cedc-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="6cedc-117">사용자는 OWA 또는 Mac 용 Outlook을 사용 하 여 공용 폴더에 계속 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6cedc-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="6cedc-118">자세한 내용은 [Outlook에서 공용 폴더에 대 한 제어 되는 연결 지원 발표](https://aka.ms/controlpf)를 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="6cedc-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>