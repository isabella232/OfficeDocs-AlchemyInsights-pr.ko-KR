---
title: 사서함의 주소 전달 확인
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 17/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 1b0a6c8fe368196f2d1f9811aea895c2c024b2e6
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50465086"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="e1332-102">사서함의 주소 전달 확인</span><span class="sxs-lookup"><span data-stu-id="e1332-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="e1332-103">경우에 따라 해커가 사용자의 전자 메일 메시지를 자신에게 전달하기 때문에 먼저 사서함의 전달 주소 및 규칙을 확인하게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="e1332-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="e1332-104">그런 다음 감사 로그를 검사합니다.</span><span class="sxs-lookup"><span data-stu-id="e1332-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="e1332-105">전달 주소를 확인하는 방법에는 다음이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e1332-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="e1332-106">사용자 **활성 사용자를**  >  **선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="e1332-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="e1332-107">계정이 손상된 사용자를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="e1332-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="e1332-108">플라이아웃이 나타나면 메일 설정 을 확장하고 전자 메일 **전달에** 대해 **편집을 클릭합니다.**</span><span class="sxs-lookup"><span data-stu-id="e1332-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="e1332-109">인식할 수 없는 전달 주소를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="e1332-109">Remove any forwarding addresses you don't recognize.</span></span>