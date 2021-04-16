---
title: 공용 폴더 사용 권한 설정 또는 변경
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: e419c72a890e68fc7b6d40d2b64406e42f9b0769
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51789213"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="8d33f-102">사용 권한 및 공용 폴더</span><span class="sxs-lookup"><span data-stu-id="8d33f-102">Permissions and Public Folders</span></span>

<span data-ttu-id="8d33f-103">Outlook, EAC(Exchange 관리 센터) 또는 PowerShell을 사용하여 공용 폴더에 대한 사용 권한을 변경할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8d33f-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="8d33f-104">Outlook 지침에 대해 [여기를 클릭합니다.](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx)</span><span class="sxs-lookup"><span data-stu-id="8d33f-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="8d33f-105">EAC의 경우 이 문서를 [참조하여](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) 지침을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="8d33f-105">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions.</span></span> 
    
- <span data-ttu-id="8d33f-106">Powershell의 경우 [](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) 이 문서에서 Add-PublicFolderClientPermission 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="8d33f-106">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet.</span></span> <span data-ttu-id="8d33f-107">Exchange Powershell에 연결하는 데 필요한 지침이 필요한 경우 여기를 [클릭합니다.](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx)</span><span class="sxs-lookup"><span data-stu-id="8d33f-107">If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="8d33f-108">외부 **사용자가** 메일 사용이 가능한 공용 폴더로 전자 메일을 보낼 수 없는 경우 공용 폴더에 외부 전자 메일 배달에 필요한 사용 권한이 누락된 것일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8d33f-108">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery.</span></span> <span data-ttu-id="8d33f-109">여기에서 Outlook 지침 또는 [](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)PowerShell 지침을 사용하여 이 문제를 해결할 수 [있습니다.](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx)</span><span class="sxs-lookup"><span data-stu-id="8d33f-109">You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

