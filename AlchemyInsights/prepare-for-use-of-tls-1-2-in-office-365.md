---
title: Microsoft 365에서 TLS 1.2 사용 준비
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Critical
ms.custom:
- "1266"
- "1600052"
ms.assetid: d5c84f5c-a3ca-4abd-8633-7e9ff01328a9
ms.openlocfilehash: 1ec40ba36c69296298e24dca64a873d53682833a
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085910"
---
# <a name="prepare-for-use-of-tls-12-in-microsoft-365"></a><span data-ttu-id="740f1-102">Microsoft 365에서 TLS 1.2 사용 준비</span><span class="sxs-lookup"><span data-stu-id="740f1-102">Prepare for use of TLS 1.2 in Microsoft 365</span></span>

<span data-ttu-id="740f1-103">2018년 10월 31일부터 Microsoft 365가 TLS 1.2로 계속해서 전환됩니다.</span><span class="sxs-lookup"><span data-stu-id="740f1-103">As of October 31st, 2018, Microsoft 365 will continue transitioning to TLS 1.2.</span></span> <span data-ttu-id="740f1-104">2020년 10월 15일부터 O365는 서비스 전반에서 TLS 1.0 및 1.1의 비호출을 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="740f1-104">Starting October 15, 2020, O365 will begin the deprecation of TLS 1.0 and 1.1 across the service.</span></span> <span data-ttu-id="740f1-105">이러한 변경에 대한 배포는 향후 몇 주 및 몇 개월 동안 계속될 것이지만, 고객은 2020년 10월 15일부터 O365에 참여할 때 TLS 1.0/1.1 호출이 작동하지 않을 것으로 가정해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="740f1-105">The rollout of this change will continue over the next few weeks and months, but customers should assume no TLS 1.0/1.1 calls will work when engaging with O365 starting Oct 15, 2020.</span></span> <span data-ttu-id="740f1-106">앞서 전달된 대로(2017년 12월 MC126199, 2018년 2월 MC128929, 2019년 7월 MC186827, 2020년 7월 MC218794) 모든 온라인 서비스를 TLS(전송 계층 보안) 1.2+로 전환하여 동급 최강의 암호화를 제공하고, 기본적으로 서비스의 보안을 강화하고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="740f1-106">As previously communicated (MC126199 in Dec 2017, MC128929 in Feb 2018, MC186827 in July 2019, and MC218794 in July 2020), we are moving all of our online services to Transport Layer Security (TLS) 1.2+ to provide best-in-class encryption, and to ensure our service is more secure, by default.</span></span> <span data-ttu-id="740f1-107">고객은 서버 및 리소스에 TLS 1.0/1.1을 계속 사용할 수 있지만 O365 리소스와 상호 작용할 때는 TLS 1.2 이상만 작동한다고 가정해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="740f1-107">Customers can still choose to have TLS 1.0/1.1 on their servers and resources, but they should assume only TLS 1.2 or higher will work when interacting with O365 resources.</span></span>
  
<span data-ttu-id="740f1-108">이러한 변경 사항에 대한 자세한 내용은 [여기](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) 및 [여기](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide)를 참조하시기 바랍니다.</span><span class="sxs-lookup"><span data-stu-id="740f1-108">To learn more about these changes, please see [here](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) and [here](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide).</span></span>

  