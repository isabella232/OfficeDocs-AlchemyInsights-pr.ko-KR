---
title: 공용 폴더 사용 권한 설정 또는 변경
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: c035d56ffade45cc4360a1d0dfca4c63bf110a38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771178"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="041fe-102">사용 권한 및 공용 폴더</span><span class="sxs-lookup"><span data-stu-id="041fe-102">Permissions and Public Folders</span></span>

<span data-ttu-id="041fe-103">Outlook, EAC (Exchange 관리 센터) 또는 PowerShell을 사용 하 여 공용 폴더에 대 한 사용 권한을 변경할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="041fe-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="041fe-104">Outlook 지침을 보려면 [여기를 클릭](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx)하십시오.</span><span class="sxs-lookup"><span data-stu-id="041fe-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="041fe-105">EAC에 대 한 자세한 내용은 [이 문서](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) 를 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="041fe-105">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions.</span></span> 
    
- <span data-ttu-id="041fe-106">Powershell의 경우에는 [이 문서](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) 에서 추가-PublicFolderClientPermission를 사용 하는 방법에 대 한 지침을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="041fe-106">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet.</span></span> <span data-ttu-id="041fe-107">Exchange Powershell에 연결 하기 위한 지침이 필요한 경우 [여기](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx)를 클릭 하십시오.</span><span class="sxs-lookup"><span data-stu-id="041fe-107">If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="041fe-108">**외부 사용자가 메일 사용이 가능한 공용 폴더에 전자 메일을 보낼 수 없는**경우 외부 전자 메일 배달에 필요한 사용 권한이 공용 폴더에 없는 이유가 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="041fe-108">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery.</span></span> <span data-ttu-id="041fe-109">[여기에서 Outlook 지침 또는](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1) [PowerShell 지침을](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx)사용 하 여이 문제를 해결할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="041fe-109">You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

