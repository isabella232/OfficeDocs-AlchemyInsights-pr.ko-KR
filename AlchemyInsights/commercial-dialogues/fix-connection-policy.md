---
title: 연결 정책 수정
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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737829"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="c04e8-102">연결 정책 수정</span><span class="sxs-lookup"><span data-stu-id="c04e8-102">Fix connection policy</span></span>

<span data-ttu-id="c04e8-103">보내는 IP 주소가 연결 필터 정책에서 안전한 것으로 표시되어 전자 메일이 안전한 것으로 표시되어 사용자의 받은 편지함으로 배달됩니다.</span><span class="sxs-lookup"><span data-stu-id="c04e8-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="c04e8-104">정책을 검토하기 위해 다음을 합니다.</span><span class="sxs-lookup"><span data-stu-id="c04e8-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="c04e8-105">[Office 365 보안](https://go.microsoft.com/fwlink/p/?linkid=2077143)& 준수 센터로 이동한 다음 위협 관리 정책 스팸 방지 로  >    >  [이동 합니다.](https://go.microsoft.com/fwlink/?linkid=2101518)</span><span class="sxs-lookup"><span data-stu-id="c04e8-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="c04e8-106">사용자 지정 **탭에서** 연결 필터 **정책 을** 선택한 다음 정책 **편집 을 선택합니다.**</span><span class="sxs-lookup"><span data-stu-id="c04e8-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="c04e8-107">IP 허용 **목록을 검토합니다.**</span><span class="sxs-lookup"><span data-stu-id="c04e8-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="c04e8-108">안전한 **목록이 사용하도록 설정되어 있는지** 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="c04e8-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="c04e8-109">Microsoft는 신뢰할 수 있는 보낸 사람에 대한 타사 소스를 구독합니다.</span><span class="sxs-lookup"><span data-stu-id="c04e8-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="c04e8-110">수신 **가능 목록이** 사용하도록 설정되어 있는 경우 이러한 신뢰할 수 있는 보낸 사람이 스팸으로 잘못 표시되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="c04e8-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="c04e8-111">받는 가음성(스팸으로 분류된 좋은 메일)의 수가 줄어들기 때문에 이 옵션을 선택하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="c04e8-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
