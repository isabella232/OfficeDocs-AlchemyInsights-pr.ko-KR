---
title: 사용자 정책/사서함 설정 수정
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568568"
---
# <a name="fix-user-policymailbox-settings"></a><span data-ttu-id="3ff6b-102">사용자 정책/사서함 설정 수정</span><span class="sxs-lookup"><span data-stu-id="3ff6b-102">Fix user policy/mailbox settings</span></span>

<span data-ttu-id="3ff6b-103">사서함의 정크 메일 설정이 이 메시지에 영향을 주었다.</span><span class="sxs-lookup"><span data-stu-id="3ff6b-103">The junk mail settings on the mailbox affected this message.</span></span> <span data-ttu-id="3ff6b-104">설정을 검토하려면 다음을 합니다.</span><span class="sxs-lookup"><span data-stu-id="3ff6b-104">To review the settings, do the following:</span></span>

1. <span data-ttu-id="3ff6b-105">Exchange 관리 셸을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="3ff6b-105">Launch Exchange Management Shell.</span></span> <span data-ttu-id="3ff6b-106">자세한 내용은 Exchange 관리 셸 [열기 를 참조하세요.](https://go.microsoft.com/fwlink/?linkid=2101432)</span><span class="sxs-lookup"><span data-stu-id="3ff6b-106">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
2. <span data-ttu-id="3ff6b-107">다음 명령을 실행합니다(사용자의 전자 메일 주소 사용):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span><span class="sxs-lookup"><span data-stu-id="3ff6b-107">Run this command (using the user's email address):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span></span>
3. <span data-ttu-id="3ff6b-108">보낸 사람 전자 메일 주소가 **TrustedSendersAndDomains** 또는 **BlockedSendersAndDomains의 일부인지 확인**</span><span class="sxs-lookup"><span data-stu-id="3ff6b-108">Check if the sender's email address is part of **TrustedSendersAndDomains** or **BlockedSendersAndDomains**.</span></span> <span data-ttu-id="3ff6b-109">전자 메일 주소가 목록 중 하나에 있는 경우 해당 주소를 제거해야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="3ff6b-109">If the email address is in one of the lists, you may have to remove it.</span></span> <span data-ttu-id="3ff6b-110">자세한 내용은 [Set-MailboxJunkEmailConfiguration을 참조합니다.](https://go.microsoft.com/fwlink/?linkid=2101047)</span><span class="sxs-lookup"><span data-stu-id="3ff6b-110">To learn more, see [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span></span>
