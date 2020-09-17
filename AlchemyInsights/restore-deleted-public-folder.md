---
title: 삭제 된 공용 폴더 복원
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
- "3488"
ms.openlocfilehash: bb7fe248714e9a7e7f4c48913b159b5c23132192
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774537"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="e4ca4-102">삭제 된 공용 폴더 복원</span><span class="sxs-lookup"><span data-stu-id="e4ca4-102">Restore a deleted public folder</span></span>

<span data-ttu-id="e4ca4-103">**공용 폴더에서 삭제 된 항목을 복원 하려면 다음을 수행 합니다**.</span><span class="sxs-lookup"><span data-stu-id="e4ca4-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="e4ca4-104">[Outlook 2016의 메일 이외의 공용 폴더에서는 삭제 된 항목을 복구할 수 없습니다](https://aka.ms/pfrec).를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="e4ca4-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="e4ca4-105">**삭제 된 공용 폴더 (모든 유형)를 복원 하려면 다음을**수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="e4ca4-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="e4ca4-106">다음 EXO PowerShell 명령을 사용 하세요.</span><span class="sxs-lookup"><span data-stu-id="e4ca4-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="e4ca4-107">구문:</span><span class="sxs-lookup"><span data-stu-id="e4ca4-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="e4ca4-108">예: 다음 명령은 Subfolder1를 복원 하 고 \Parent1 아래에 배치 합니다.</span><span class="sxs-lookup"><span data-stu-id="e4ca4-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="e4ca4-109">자세한 내용은 [삭제 된 공용 폴더 복원을](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="e4ca4-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
