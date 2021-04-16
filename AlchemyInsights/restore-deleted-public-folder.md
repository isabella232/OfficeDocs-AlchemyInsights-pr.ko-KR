---
title: 삭제된 공용 폴더 복원
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
- "3488"
ms.openlocfilehash: d5480389c3bf50cee9fe30f7ec8d8ff28ef694ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809445"
---
# <a name="restore-a-deleted-public-folder"></a>삭제된 공용 폴더 복원

**공용 폴더에서 삭제된 항목을 복원하려면**:

- [Outlook 2016에서](https://aka.ms/pfrec)메일이 없는 공용 폴더에서 삭제된 항목을 복구할 수 없습니다를 참조합니다.
 
삭제된 공용 폴더(모든 **형식)를 복원하려면**: 

- 다음 EXO PowerShell 명령을 사용하시기 바랍니다.

    구문:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    예: 다음 명령은 Subfolder1을 복원하고 \Parent1 아래에 를 습니다.

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

자세한 [내용은 삭제된](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) 공용 폴더 복원을 참조합니다.
