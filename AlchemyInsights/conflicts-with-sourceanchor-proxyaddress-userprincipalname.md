---
title: 원본 앵커, ProxyAddress, UserPrincipalName와 충돌합니다.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1699"
- "1300022"
ms.openlocfilehash: 826dfe9e5c7d24ff5186a94e1ada4dad536e7edd
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/20/2020
ms.locfileid: "45186127"
---
# <a name="conflicts-with-sourceanchor-proxyaddress-userprincipalname"></a><span data-ttu-id="6754e-102">원본 앵커, ProxyAddress, UserPrincipalName와 충돌합니다.</span><span class="sxs-lookup"><span data-stu-id="6754e-102">Conflicts with SourceAnchor, ProxyAddress, UserPrincipalName</span></span>

<span data-ttu-id="6754e-103">"디렉토리에 동일한 ProxyAddress 또는 UserPrincipalName를 사용하는 동기화 된 개체가 있습니다"와 같은 동기화 중에 오류 메시지가 발생 하는 경우 [중복 특성 동기화 오류 진단 및 해결](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors)을참조하세요.</span><span class="sxs-lookup"><span data-stu-id="6754e-103">If you receive errors during a synchronization such as "A synchronized object with the same ProxyAddress or UserPrincipalName exists in your directory", see [Diagnose and remediate duplicated attribute sync errors](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span></span>

<span data-ttu-id="6754e-104">또한 중복 특성 복구를 사용 하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="6754e-104">Also, consider enabling duplicate attribute resiliency.</span></span> <span data-ttu-id="6754e-105">자세한 내용은 [ID 동기화 및 중복 특성 복구](https://aka.ms/duplicateattributeresiliency)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="6754e-105">For more info, see [Identity synchronization and duplicate attribute resiliency](https://aka.ms/duplicateattributeresiliency).</span></span>