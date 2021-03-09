---
title: 테넌트 정책 수정(작업 오버라이드)
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50552436"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="6e5d0-102">테넌트 정책 수정(작업 오버라이드)</span><span class="sxs-lookup"><span data-stu-id="6e5d0-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="6e5d0-103">테넌트의 스팸 방지 정책이 이 메시지에 영향을 주었다.</span><span class="sxs-lookup"><span data-stu-id="6e5d0-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="6e5d0-104">정책을 검토하기 위해 다음을 합니다.</span><span class="sxs-lookup"><span data-stu-id="6e5d0-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="6e5d0-105">[Office 365 보안](https://go.microsoft.com/fwlink/p/?linkid=2077143)& 준수 센터로 이동한 다음 위협 관리 정책 스팸 방지 로  >    >  [이동 합니다.](https://go.microsoft.com/fwlink/?linkid=2101518)</span><span class="sxs-lookup"><span data-stu-id="6e5d0-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="6e5d0-106">정책 **원본에** 다음이 나타내는지  **확인: Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC 메시지**</span><span class="sxs-lookup"><span data-stu-id="6e5d0-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="6e5d0-107">그렇다면 사용자 지정 **탭에서** 메시지에 영향을 주는 정책의 설정을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="6e5d0-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="6e5d0-108">모든 Exchange Online Protection 고객에게 **적용된 표준** 설정이 메시지에 영향을 줄 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="6e5d0-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="6e5d0-109">스팸 필터 정책 구성에 대한 자세한 내용은 스팸 필터 정책 [구성을 참조하세요.](https://go.microsoft.com/fwlink/?linkid=2101431)</span><span class="sxs-lookup"><span data-stu-id="6e5d0-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>
