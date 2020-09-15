---
title: Outlook을 사용하여 공용 폴더에 대한 액세스 제어하기
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 4ef62fe8c9cc438c48ed8897a8b3385b15669cdc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680488"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="1dd70-102">Outlook을 사용하여 공용 폴더에 대한 액세스 제어하기</span><span class="sxs-lookup"><span data-stu-id="1dd70-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="1dd70-103">Outlook을 사용하여 공용 폴더에 액세스할 수 있는 사용자를 제어하려면:</span><span class="sxs-lookup"><span data-stu-id="1dd70-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="1dd70-104">`Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false` 사용</span><span class="sxs-lookup"><span data-stu-id="1dd70-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="1dd70-105">$true: Outlook의 공용 폴더에 대한 사용자 액세스 허용</span><span class="sxs-lookup"><span data-stu-id="1dd70-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="1dd70-106">$false: Outlook의 공용 폴더에 대한 사용자 액세스 차단</span><span class="sxs-lookup"><span data-stu-id="1dd70-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="1dd70-107">이 값은 기본값입니다.</span><span class="sxs-lookup"><span data-stu-id="1dd70-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="1dd70-108">참고: 이 절차는 Windows 클라이언트용 Outlook 데스크톱과의 연결만 제어합니다.</span><span class="sxs-lookup"><span data-stu-id="1dd70-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="1dd70-109">사용자는 OWA 또는 Mac용 Outlook을 사용하여 공용 폴더에 계속 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="1dd70-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="1dd70-110">자세한 내용은 [Outlook의 공용 폴더에 대한 제어된 연결](https://aka.ms/controlpf)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="1dd70-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
