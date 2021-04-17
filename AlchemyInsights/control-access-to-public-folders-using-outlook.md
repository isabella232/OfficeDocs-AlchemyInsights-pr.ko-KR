---
title: Outlook을 사용하여 공용 폴더에 대한 액세스 제어하기
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816746"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="a7799-102">Outlook을 사용하여 공용 폴더에 대한 액세스 제어하기</span><span class="sxs-lookup"><span data-stu-id="a7799-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="a7799-103">Outlook을 사용하여 공용 폴더에 액세스할 수 있는 사용자를 제어하려면:</span><span class="sxs-lookup"><span data-stu-id="a7799-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="a7799-104">`Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false` 사용</span><span class="sxs-lookup"><span data-stu-id="a7799-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="a7799-105">$true: Outlook의 공용 폴더에 대한 사용자 액세스 허용</span><span class="sxs-lookup"><span data-stu-id="a7799-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="a7799-106">$false: Outlook의 공용 폴더에 대한 사용자 액세스 차단</span><span class="sxs-lookup"><span data-stu-id="a7799-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="a7799-107">이 값은 기본값입니다.</span><span class="sxs-lookup"><span data-stu-id="a7799-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="a7799-108">참고: 이 절차는 Windows 클라이언트용 Outlook 데스크톱과의 연결만 제어합니다.</span><span class="sxs-lookup"><span data-stu-id="a7799-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="a7799-109">사용자는 OWA 또는 Mac용 Outlook을 사용하여 공용 폴더에 계속 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a7799-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="a7799-110">자세한 내용은 [Outlook의 공용 폴더에 대한 제어된 연결](https://aka.ms/controlpf)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="a7799-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
