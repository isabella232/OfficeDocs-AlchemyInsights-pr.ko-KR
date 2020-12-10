---
title: Microsoft Edge 사용자 에이전트 문자열(데스크톱)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003862"
- "6914"
ms.openlocfilehash: b4106dde1e09e0ce07b4b9adc2b2984cc5609c3b
ms.sourcegitcommit: 3c6e777d6679a24108171e9aa3f9379a8d44e001
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49609677"
---
# <a name="microsoft-edge-user-agent-string-desktop"></a><span data-ttu-id="950c8-102">Microsoft Edge 사용자 에이전트 문자열(데스크톱)</span><span class="sxs-lookup"><span data-stu-id="950c8-102">Microsoft Edge user agent string (Desktop)</span></span>

<span data-ttu-id="950c8-103">UA(사용자 에이전트) 문자열을 사용하여 특정 운영 체제에서 사용되고 있는 특정 브라우저 버전을 검색할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="950c8-103">User agent (UA) strings can be used to detect what version of a specific browser is being used on a certain operating system.</span></span> <span data-ttu-id="950c8-104">다른 브라우저와 마찬가지로 Microsoft Edge는 사이트에 대한 요청을 할 때마다 "User-Agent" HTTP 헤더에 이 정보를 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="950c8-104">Like other browsers, Microsoft Edge includes this information in the "User-Agent" HTTP header whenever it makes a request to a site.</span></span> <span data-ttu-id="950c8-105">"navigator.userAgent" 값을 쿼리하여 JavaScript를 통해 브라우저 버전 정보에 액세스할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="950c8-105">The browser-version information can also be accessed via JavaScript by querying the value of "navigator.userAgent".</span></span>

<span data-ttu-id="950c8-106">웹 개발자는 가능한 경우 기능 검색을 사용하여 코드 유지 관리 성능을 향상하고, 코드 취약성을 줄이고, 향후 UA 문자열 업데이트 시 코드 중단 위험을 제거하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="950c8-106">We recommend that web developers make use of feature detection whenever possible to improve code maintainability, reduce code fragility, and eliminate the risk of code breakage in the event of future UA string updates.</span></span>

<span data-ttu-id="950c8-107">자세한 내용은 Microsoft Edge 사용자 에이전트 [문자열(데스크톱)을 참조하세요.](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string)</span><span class="sxs-lookup"><span data-stu-id="950c8-107">For more information, see [Microsoft Edge User Agent String (Desktop)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).</span></span>