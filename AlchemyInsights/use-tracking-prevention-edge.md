---
title: Microsoft Edge(Chromium)에서 추적 방지 사용
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8328"
- "9004625"
ms.openlocfilehash: 09e9a7303063328cd7bd0a0fcbf9629a3b38ebb5
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51408787"
---
# <a name="use-tracking-prevention-in-microsoft-edge-chromium"></a><span data-ttu-id="f56d4-102">Microsoft Edge(Chromium)에서 추적 방지 사용</span><span class="sxs-lookup"><span data-stu-id="f56d4-102">Use tracking prevention in Microsoft Edge (Chromium)</span></span>

<span data-ttu-id="f56d4-103">Microsoft Edge의 추적 방지는 트래커가 브라우저 기반 저장소 및 네트워크에 액세스하는 기능을 제한합니다.</span><span class="sxs-lookup"><span data-stu-id="f56d4-103">Tracking prevention in Microsoft Edge limits a tracker's ability to access browser-based storage and the network.</span></span> <span data-ttu-id="f56d4-104">이 기능은 Microsoft Edge를 사용하는 사용자가 웹에서 안전할 수 있도록 지원하겠다는 당사의 약속을 지키기 위해 구축되었습니다.</span><span class="sxs-lookup"><span data-stu-id="f56d4-104">The feature is built to uphold our commitment to helping users stay safe on the web with Microsoft Edge.</span></span> <span data-ttu-id="f56d4-105">개인 정보자세한 내용은 [Microsoft Edge(Chromium)에서 추적 방지](https://go.microsoft.com/fwlink/?linkid=2135435) 및 [Microsoft의 브라우저 개인 정보 보호 약속](https://go.microsoft.com/fwlink/?linkid=2135350)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="f56d4-105">For more information, see [Tracking prevention in Microsoft Edge (Chromium)](https://go.microsoft.com/fwlink/?linkid=2135435) and [Our browser privacy promise](https://go.microsoft.com/fwlink/?linkid=2135350).</span></span>

<span data-ttu-id="f56d4-106">Microsoft Edge에서는 edge://settings/privacy에서 선택할 수 있는 세 가지 수준의 추적 방지 기능을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="f56d4-106">Microsoft Edge offers three levels of tracking prevention (they can be selected in edge://settings/privacy):</span></span>

- <span data-ttu-id="f56d4-107">**기본** 은 가장 덜 제한적이며, 개인 설정된 광고를 즐기고 웹에서 추적되는 것에 개의치 않는 사용자를 위해 설계되었습니다.</span><span class="sxs-lookup"><span data-stu-id="f56d4-107">**Basic** is the least restrictive and designed for users who enjoy personalized advertisements and don't mind being tracked on the web.</span></span> <span data-ttu-id="f56d4-108">기본은 핑거프린터 및 크립토마이너 같은 악의적인 트래커로부터만 사용자를 보호합니다.</span><span class="sxs-lookup"><span data-stu-id="f56d4-108">Basic protects users only against malicious trackers, such as fingerprinters and cryptominers.</span></span>
- <span data-ttu-id="f56d4-109">**균형 잡힌** 수준은 기본 수준으로, 웹 광고 수를 줄이려 하는 사용자를 위해 설계되었습니다.</span><span class="sxs-lookup"><span data-stu-id="f56d4-109">**Balanced** is the default level and designed for users who want to see fewer advertisements that follow them around the web.</span></span> <span data-ttu-id="f56d4-110">균형 잡힌 수준은 사용자가 참여하지 않는 사이트의 트래커를 차단할 뿐만 아니라 호환성 문제의 위험을 최소화하는 것도 목표로 합니다.</span><span class="sxs-lookup"><span data-stu-id="f56d4-110">Balanced level aims not only to block trackers from sites that users never engage with but also to minimize the risk of compatibility issues.</span></span>
- <span data-ttu-id="f56d4-111">**엄격한** 수준은 가장 제한적이며, 최대 개인 정보 보호를 위해 웹 사이트 호환성도 희생할 수 있는 사용자를 위해 설계되었습니다.</span><span class="sxs-lookup"><span data-stu-id="f56d4-111">**Strict** is the most restrictive and designed for users who don't mind sacrificing website compatibility for maximum privacy.</span></span>