---
title: Office의 이전 빌드로 롤백
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1741"
- "9000140"
ms.openlocfilehash: 8c7d019ec1aa6c26cffebbcd2c3e5751c853e3a4
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431751"
---
# <a name="roll-back-to-an-earlier-build-of-office"></a><span data-ttu-id="031e8-102">Office의 이전 빌드로 롤백</span><span class="sxs-lookup"><span data-stu-id="031e8-102">Roll back to an earlier build of Office</span></span>

<span data-ttu-id="031e8-103">이전의 Microsoft 365 앱 빌드 또는 버전으로 돌아가려면 [이전 버전의 Office로 되돌리는 방법](https://support.microsoft.com/help/2770432/how-to-revert-to-an-earlier-version-of-office-2013-or-office-2016-clic)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="031e8-103">To revert to an earlier Microsoft 365 Apps build or version, see [How to revert to an earlier version of Office](https://support.microsoft.com/help/2770432/how-to-revert-to-an-earlier-version-of-office-2013-or-office-2016-clic).</span></span> <span data-ttu-id="031e8-104">Microsoft 365 구독에서 다른 구독으로 전환 하려면  [다른 비즈니스용 Microsoft 365 요금제로 전환](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="031e8-104">To switch from one Microsoft 365 subscription to another, see  [Switch to a different Microsoft 365 for business plan](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span></span>

- <span data-ttu-id="031e8-105">현재 사용 중인 Office 버전을 찾으려면 [무슨 Office 버전을 사용하고 있나요?](https://support.office.com/article/about-office-what-version-of-office-am-i-using-932788b8-a3ce-44bf-bb09-e334518b8b19)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="031e8-105">To find the version of Office you are currently using, see [About Office: What version of Office am I using?](https://support.office.com/article/about-office-what-version-of-office-am-i-using-932788b8-a3ce-44bf-bb09-e334518b8b19).</span></span>
- <span data-ttu-id="031e8-106">롤백할 빌드를 확인하려면 [Microsoft 365 앱 업데이트 기록(날짜 순으로 나열)](https://docs.microsoft.com/officeupdates/update-history-office365-proplus-by-date?redirectSourcePath=%252fen-us%252farticle%252fae942449-1fca-4484-898b-a933ea23def7)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="031e8-106">To determine the build you want to roll back to, see [Update history for Microsoft 365 Apps (listed by date)](https://docs.microsoft.com/officeupdates/update-history-office365-proplus-by-date?redirectSourcePath=%252fen-us%252farticle%252fae942449-1fca-4484-898b-a933ea23def7).</span></span>
- <span data-ttu-id="031e8-107">[이전 버전 Office로 롤백 하는 방법](https://support.microsoft.com/help/2770432/how-to-revert-to-an-earlier-version-of-office-2013-or-office-2016-clic) 혹은 [Office CDN(콘텐츠 배달 네트워크)를 사용하여 반기 채널에서 기능 업데이트 받기 지연](https://docs.microsoft.com/deployoffice/delay-receiving-feature-updates-from-deferred-channel-for-office-365-proplus#delay-receiving-feature-updates-from-semi-annual-channel-when-using-the-office-content-delivery-network-cdn)을 사용하여 이전 빌드로 돌아가기 위한 **TargetVersion** 설정을 구성합니다.</span><span class="sxs-lookup"><span data-stu-id="031e8-107">Configure the **TargetVersion** setting to revert to the earlier build by using [How to revert to an earlier version of Office](https://support.microsoft.com/help/2770432/how-to-revert-to-an-earlier-version-of-office-2013-or-office-2016-clic) or [Delay receiving feature updates from Semi-Annual Channel when using the Office Content Delivery Network (CDN)](https://docs.microsoft.com/deployoffice/delay-receiving-feature-updates-from-deferred-channel-for-office-365-proplus#delay-receiving-feature-updates-from-semi-annual-channel-when-using-the-office-content-delivery-network-cdn).</span></span></br>
    <span data-ttu-id="031e8-108">대상 버전을 설정하면 Office가 다음번에 업데이트를 확인할 때 해당 버전으로 업데이트 합니다.</span><span class="sxs-lookup"><span data-stu-id="031e8-108">When the target version is set, Office updates to that version the next time it looks for updates.</span></span>