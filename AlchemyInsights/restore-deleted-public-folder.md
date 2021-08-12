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
ms.openlocfilehash: 6df196fc0bde37c962e3aa84dd602ee414dad3d329addfd16cb6e3dcc40fc2ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53943381"
---
# <a name="restore-a-deleted-public-folder"></a>삭제된 공용 폴더 복원

**공용 폴더에서 삭제된 항목을 복원하려면**:

- 에서 메일이 없는 공용 폴더에서 삭제된 항목을 [복구할 수 Outlook 2016.](https://aka.ms/pfrec)
 
삭제된 공용 폴더(모든 **형식)를 복원하려면**: 

- 다음 EXO PowerShell 명령을 사용하시기 바랍니다.

    구문:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    예: 다음 명령은 Subfolder1을 복원하고 \Parent1 아래에 를 습니다.

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

자세한 [내용은 삭제된](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) 공용 폴더 복원을 참조합니다.
