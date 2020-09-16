---
title: Ediscovery 내보내기용 Chromium 브라우저에 따라 Microsoft Edge 사용
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3473"
- "3100022"
ms.openlocfilehash: 64aebb7f048dba37eef8cd1fa6286b36823d3f0f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734521"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a><span data-ttu-id="47c62-102">Ediscovery 내보내기용 Chromium 브라우저에 따라 Microsoft Edge 사용</span><span class="sxs-lookup"><span data-stu-id="47c62-102">Using Microsoft Edge based on Chromium browsers for Ediscovery export</span></span>

<span data-ttu-id="47c62-103">최근 변경 사항으로 인해 Microsoft Edge 브라우저에서는 더 이상 ClickOnce 지원 기능이 기본적으로 사용 되지 않도록 설정 됩니다.</span><span class="sxs-lookup"><span data-stu-id="47c62-103">Due to a recent change, Microsoft Edge browsers will no longer have ClickOnce support enabled by default.</span></span> <span data-ttu-id="47c62-104">Microsoft 365 eDiscovery 내보내기 도구를 계속 사용 하려면 microsoft Internet Explorer를 사용 하거나 Microsoft Edge에서 ClickOnce 지원을 사용 하도록 설정 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="47c62-104">To continue using the Microsoft 365 eDiscovery Export Tool, you will either need to use Microsoft Internet Explorer or enable ClickOnce Support in Microsoft Edge.</span></span> 

<span data-ttu-id="47c62-105">Chromium를 기반으로 Microsoft Edge에서 ClickOnce 지원을 사용 하도록 설정 하려면 다음을 수행 합니다.</span><span class="sxs-lookup"><span data-stu-id="47c62-105">To enable ClickOnce Support in Microsoft Edge based on Chromium:</span></span> 
1. <span data-ttu-id="47c62-106">Microsoft Edge 브라우저에서 edge://flags/을 한 번 클릭 하 여 #edge를 방문 합니다.</span><span class="sxs-lookup"><span data-stu-id="47c62-106">In your Microsoft Edge browser, visit edge://flags/#edge-click-once.</span></span>
2. <span data-ttu-id="47c62-107">ClickOnce 지원 옵션에 대해 값을 **기본값** 또는 **사용 안 함** 에서 **사용**으로 변경 합니다.</span><span class="sxs-lookup"><span data-stu-id="47c62-107">For the ClickOnce Support option, change the value from **Default** or **Disabled** to **Enabled**.</span></span> 
3. <span data-ttu-id="47c62-108">브라우저 창 아래쪽에서 **다시 시작**을 선택 합니다.</span><span class="sxs-lookup"><span data-stu-id="47c62-108">At the bottom of the browser window, select **Restart**.</span></span> <br>
 <span data-ttu-id="47c62-109">변경 내용을 적용 하려면 Microsoft Edge를 다시 시작 해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="47c62-109">The change will take effect after restarting Microsoft Edge.</span></span> 

<span data-ttu-id="47c62-110">이에 대 한 자세한 내용과 내보내기 도구를 설치 하는 단계는: [ 콘텐츠 검색 결과 내보내기](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="47c62-110">For information on this and steps for installing the  export tool, see: [ Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>