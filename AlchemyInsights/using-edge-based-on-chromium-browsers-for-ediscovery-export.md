---
title: Ediscovery 내보내기용 Chromium 브라우저 기반 Microsoft Edge 사용
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3473"
- "3100022"
ms.openlocfilehash: 7ee724e5109effce8883be50e360948313c84b34
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834377"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a><span data-ttu-id="41e04-102">Ediscovery 내보내기용 Chromium 브라우저 기반 Microsoft Edge 사용</span><span class="sxs-lookup"><span data-stu-id="41e04-102">Using Microsoft Edge based on Chromium browsers for Ediscovery export</span></span>

<span data-ttu-id="41e04-103">최근 변경으로 인해 Microsoft Edge 브라우저는 더 이상 ClickOnce 지원이 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="41e04-103">Due to a recent change, Microsoft Edge browsers will no longer have ClickOnce support enabled by default.</span></span> <span data-ttu-id="41e04-104">Microsoft 365 eDiscovery 내보내기 도구를 계속 사용하려면 Microsoft Edge에서 Microsoft Internet Explorer ClickOnce 사용하도록 설정해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="41e04-104">To continue using the Microsoft 365 eDiscovery Export Tool, you will either need to use Microsoft Internet Explorer or enable ClickOnce Support in Microsoft Edge.</span></span> 

<span data-ttu-id="41e04-105">Chromium을 ClickOnce Microsoft Edge에서 지원이 가능하도록 설정하려면</span><span class="sxs-lookup"><span data-stu-id="41e04-105">To enable ClickOnce Support in Microsoft Edge based on Chromium:</span></span> 
1. <span data-ttu-id="41e04-106">Microsoft Edge 브라우저에서 웹 사이트를 edge://flags/#edge-click-once.</span><span class="sxs-lookup"><span data-stu-id="41e04-106">In your Microsoft Edge browser, visit edge://flags/#edge-click-once.</span></span>
2. <span data-ttu-id="41e04-107">ClickOnce 지원 옵션의 경우 **기본** 또는 **사용하지 않음** 에서 **사용함** 으로 값을 변경할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="41e04-107">For the ClickOnce Support option, change the value from **Default** or **Disabled** to **Enabled**.</span></span> 
3. <span data-ttu-id="41e04-108">At the bottom of the browser window, select **Restart**.</span><span class="sxs-lookup"><span data-stu-id="41e04-108">At the bottom of the browser window, select **Restart**.</span></span> <br>
 <span data-ttu-id="41e04-109">변경은 Microsoft Edge를 다시 시작한 후에 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="41e04-109">The change will take effect after restarting Microsoft Edge.</span></span> 

<span data-ttu-id="41e04-110">이 내용 및 내보내기 도구를 설치하는 단계에 대한 자세한 내용은 Export Content Search results (콘텐츠 검색 결과 [내보내기)를 참조하세요.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)</span><span class="sxs-lookup"><span data-stu-id="41e04-110">For information on this and steps for installing the  export tool, see: [ Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>