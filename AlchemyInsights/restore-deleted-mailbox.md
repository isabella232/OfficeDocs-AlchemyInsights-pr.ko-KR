---
title: 삭제 된 사서함 복원
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "360"
- "3500005"
search.appverid:
- MOE150
- MED150
- MBS150
ms.assetid: e6112a76-bbb6-4c22-b2e6-690b004d92d4
ms.openlocfilehash: 284024bdf9728e8463fe69ef9c9c2695035faf2f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511370"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="71813-102">삭제된 사서함 복원</span><span class="sxs-lookup"><span data-stu-id="71813-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="71813-103">사용자가 Exchange Online 라이선스를 잃어 잃으면 해당 사서함은 30 일간 보존 되며 사용자에 게 라이선스를 다시 할당 하 여 복구할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="71813-103">When a user loses an Exchange Online license, their mailbox is retained for 30 days and can be recovered by simply re-assigning the license to the user.</span></span>
  
 <span data-ttu-id="71813-104">*이 작업은 30 일 이내에만 작동 합니다.*</span><span class="sxs-lookup"><span data-stu-id="71813-104">*This will work only within 30 days.*</span></span>  
  
1. <span data-ttu-id="71813-105">Microsoft 365 관리 센터에서 **사용자** \> **활성 사용자** 페이지로 이동 합니다.</span><span class="sxs-lookup"><span data-stu-id="71813-105">In the Microsoft 365 admin center, go to the **Users** \> **Active users** page.</span></span> <span data-ttu-id="71813-106">해당 하는 사용자를 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="71813-106">Select the user in question.</span></span>

2. <span data-ttu-id="71813-107">**라이선스 및 앱** 탭에서 Exchange Online 라이선스를 할당 하 고 **변경 내용 저장**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="71813-107">On the **Licenses and Apps** tab, assign the Exchange Online license and select **Save changes**.</span></span>

<span data-ttu-id="71813-108">공유 사서함을 복구 하려는 경우 30 일 동안에도 복구할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="71813-108">If you are trying to recover a Shared mailbox, it is also recoverable for 30 days.</span></span> <span data-ttu-id="71813-109">**사용자가** \> **삭제 된 사용자**아래에서 찾을 수 있으며, 공유 사서함에는 라이선스가 필요 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="71813-109">You can find them under **Users** \> **Deleted users**; shared mailboxes do not require a license.</span></span> <span data-ttu-id="71813-110">삭제 된 사용자를 복원 해야 하는 경우에 [는 restore a user](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="71813-110">If you realize that you need to restore a deleted user, please see [Restore a user](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
  