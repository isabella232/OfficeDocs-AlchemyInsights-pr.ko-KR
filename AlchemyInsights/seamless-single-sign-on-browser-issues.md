---
title: 원활한 SSO(Single Sign-On) 브라우저 문제 해결
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9377"
ms.openlocfilehash: 507dc5a3bdc5f1bc27cf12865daf98df6c702827
ms.sourcegitcommit: f835aa80f2d85e9c0549be9395110377dba50f3d
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50530822"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-browser-issues"></a><span data-ttu-id="bd809-102">원활한 SSO(Single Sign-On) 브라우저 문제 해결</span><span class="sxs-lookup"><span data-stu-id="bd809-102">Troubleshoot Seamless Single Sign-on (SSO) browser issues</span></span>

<span data-ttu-id="bd809-103">대부분의 사용자는 아래 단계를 사용하여 원활한 SSO 브라우저 문제를 해결할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="bd809-103">Most users are able to resolve their Seamless SSO browser issue using the steps below:</span></span>

1. <span data-ttu-id="bd809-104">브라우저를 최신으로 유지해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="bd809-104">Make sure your browser is up-to-date.</span></span>
2. <span data-ttu-id="bd809-105">브라우저에서 쿠키를 삭제하여 잘못된 SSO 세션을 제거하고 다시 로그인을 시도합니다.</span><span class="sxs-lookup"><span data-stu-id="bd809-105">Delete cookies from your browser to remove an invalid SSO session and try logging in again.</span></span>
3. <span data-ttu-id="bd809-106">다른 브라우저를 사용하여 로그인해 보십시오.</span><span class="sxs-lookup"><span data-stu-id="bd809-106">Try logging in using a different browser.</span></span>

<span data-ttu-id="bd809-107">**알려진 브라우저 문제**</span><span class="sxs-lookup"><span data-stu-id="bd809-107">**Known Browser Issues**</span></span>

- <span data-ttu-id="bd809-108">Seamless SSO는 Firefox의 개인 검색 모드에서 작동하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="bd809-108">Seamless SSO doesn't work in private browsing mode on Firefox.</span></span>
- <span data-ttu-id="bd809-109">고급 보호 모드가 켜져 있는 Internet Explorer 원활한 SSO가 작동하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="bd809-109">Seamless SSO doesn't work in Internet Explorer when Enhanced Protected mode is turned on.</span></span>
- <span data-ttu-id="bd809-110">Seamless SSO는 Microsoft Edge(레거시)의 비공개 검색 모드에서 작동하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="bd809-110">Seamless SSO doesn't work in private browsing mode on Microsoft Edge (legacy).</span></span>
- <span data-ttu-id="bd809-111">Seamless SSO는 iOS 및 Android의 모바일 브라우저에서 작동하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="bd809-111">Seamless SSO doesn't work on mobile browsers on iOS and Android.</span></span>

<span data-ttu-id="bd809-112">Seamless SSO는 Chromium을 기반으로 하는 다음 버전의 Microsoft Edge를 지원하며, InPrivate 및 게스트 모드에서는 디자인에 따라 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="bd809-112">Seamless SSO supports the next version of Microsoft Edge based on Chromium and it works in InPrivate and Guest mode by design.</span></span>

<span data-ttu-id="bd809-113">**권고**</span><span class="sxs-lookup"><span data-stu-id="bd809-113">**Advisory**</span></span>

<span data-ttu-id="bd809-114">Seamless SSO에 대한 기능 요청을 하거나 기술 질문을 묻는 내용은 [Microsoft Q&A를 참조하세요.](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html)</span><span class="sxs-lookup"><span data-stu-id="bd809-114">To make feature requests or ask technical questions about Seamless SSO, see [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html)</span></span>
