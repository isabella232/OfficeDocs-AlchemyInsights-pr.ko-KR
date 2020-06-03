---
title: Exchange 관리 센터의 보존 정책이 작동 하지 않음
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 3040365b9d686bcbcce60977ee9bdbbaffc70b24
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502613"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="ee7ba-102">Exchange 관리 센터의 보존 정책</span><span class="sxs-lookup"><span data-stu-id="ee7ba-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="ee7ba-103">**문제:** Exchange 관리 센터에서 새로 만들어지거나 업데이트 된 보존 정책이 사서함 이나 항목에 적용 되지 않으면 보관 사서함으로 이동 되거나 삭제 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="ee7ba-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="ee7ba-104">**근본 원인:**</span><span class="sxs-lookup"><span data-stu-id="ee7ba-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="ee7ba-105">**관리 되는 폴더 도우미가** 사용자 사서함을 처리 하지 않았기 때문일 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ee7ba-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="ee7ba-106">관리 되는 폴더 도우미는 8 일 마다 한 번씩 클라우드 기반 조직의 모든 사서함을 처리 하려고 시도 합니다.</span><span class="sxs-lookup"><span data-stu-id="ee7ba-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="ee7ba-107">보존 태그를 변경 하거나 사서함에 다른 보존 정책을 적용 하는 경우 관리 되는 폴더 지원에서 사서함을 처리할 때까지 기다리거나, 관리 되는 폴더 도우미를 실행 하 여 특정 사서함을 처리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ee7ba-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="ee7ba-108">이 cmdlet을 실행 하는 것은 보존 정책이 나 보존 태그 설정을 테스트 하거나 문제를 해결 하는 데 유용 합니다.</span><span class="sxs-lookup"><span data-stu-id="ee7ba-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="ee7ba-109">자세한 내용을 보려면 [관리 되는 폴더 도우미 실행](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist)을 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="ee7ba-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="ee7ba-110">**해결 방법:** 다음 명령을 실행 하 여 특정 사서함에 대 한 관리 되는 폴더 도우미를 시작 합니다.</span><span class="sxs-lookup"><span data-stu-id="ee7ba-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="ee7ba-111">사서함에 대 한 **보존 상태** 를 **사용 하도록 설정** 된 경우에도이 문제가 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="ee7ba-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="ee7ba-112">사서함이 보존 상태에 있는 경우에는 해당 시간 동안 사서함에 대 한 보관 정책이 처리 되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="ee7ba-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="ee7ba-113">보존 설정에 대 한 자세한 informaton [사서함 보존 보류](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="ee7ba-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="ee7ba-114">**솔루션**</span><span class="sxs-lookup"><span data-stu-id="ee7ba-114">**Solution:**</span></span>
    
  - <span data-ttu-id="ee7ba-115">[Exo powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)의 특정 사서함에 대 한 보존 설정의 상태를 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="ee7ba-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="ee7ba-116">다음 명령을 실행 하 여 특정 사서함의 보존 상태를 **사용 하지 않도록 설정** 합니다.</span><span class="sxs-lookup"><span data-stu-id="ee7ba-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="ee7ba-117">이제 관리 되는 폴더 도우미를 다시 실행 합니다.</span><span class="sxs-lookup"><span data-stu-id="ee7ba-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="ee7ba-118">**참고:** 사서함이 10mb 보다 작으면 관리 되는 폴더 도우미가 사서함을 자동으로 처리 하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="ee7ba-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="ee7ba-119">Exchange 관리 센터의 보존 정책에 대 한 자세한 내용은 다음 항목을 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="ee7ba-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="ee7ba-120">보존 태그 및 보존 정책</span><span class="sxs-lookup"><span data-stu-id="ee7ba-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="ee7ba-121">사서함에 보존 정책 적용</span><span class="sxs-lookup"><span data-stu-id="ee7ba-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="ee7ba-122">보존 태그 추가 또는 제거</span><span class="sxs-lookup"><span data-stu-id="ee7ba-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="ee7ba-123">사서함의 보류 유형을 식별하는 방법</span><span class="sxs-lookup"><span data-stu-id="ee7ba-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
