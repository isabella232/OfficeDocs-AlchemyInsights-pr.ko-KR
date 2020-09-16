---
title: cmdlet으로 삭제된 항목 복구
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
- "1800008"
- "5718"
ms.openlocfilehash: 91a9bcf75b13881b903a1d3b6f2da53f65811c9c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741309"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="0c78e-102">cmdlet으로 삭제된 항목 복구</span><span class="sxs-lookup"><span data-stu-id="0c78e-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="0c78e-103">[Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet을 사용해 사서함에서 삭제된 항목을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="0c78e-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="0c78e-104">삭제된 항목을 찾은 후 [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet을 사용해 삭제된 항목을 복구합니다.</span><span class="sxs-lookup"><span data-stu-id="0c78e-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="0c78e-105">[Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)에서 자세한 사항을 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="0c78e-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="0c78e-106">이 cmdlet을 실행하기 전에 사서함 가져오기 내보내기 역할이 할당되어 있어야 합니다</span><span class="sxs-lookup"><span data-stu-id="0c78e-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="0c78e-107">자세한 내용은 [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="0c78e-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
