---
title: 수동으로 Microsoft Edge에 로그인
ms.author: v-smandalika
author: v-smandalika
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9003844"
- "6893"
- "8332"
- "9004625"
ms.openlocfilehash: f380d09dc14788205638cdee6aebe0b084ecab2f
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398663"
---
# <a name="sign-in-to-microsoft-edge-manually"></a><span data-ttu-id="29cac-102">수동으로 Microsoft Edge에 로그인</span><span class="sxs-lookup"><span data-stu-id="29cac-102">Sign in to Microsoft Edge manually</span></span>

<span data-ttu-id="29cac-103">첫 실행 경험 중에 사용자가 자동으로 로그인되지 않은 경우 사용자는 브라우저 설정 또는 ID 플라이아웃을 통해 수동으로 로그인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="29cac-103">If a user isn't automatically signed in during a first-run experience, the user can manually sign in through the browser's settings or the identity flyout.</span></span> <span data-ttu-id="29cac-104">로그인을 관리하기 위해 다음 정책을 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="29cac-104">To manage sign-in, use the following policies:</span></span>

1. <span data-ttu-id="29cac-105">[NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) - 사용자가 Microsoft Edge에서 항상 작업 프로필을 사용할 수 있도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="29cac-105">[NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) - To ensure that a user always has a work profile in Microsoft Edge.</span></span>
2. <span data-ttu-id="29cac-106">[RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) - 로그인을 신뢰할 수 있는 계정 집합으로 제한합니다.</span><span class="sxs-lookup"><span data-stu-id="29cac-106">[RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) - To restrict sign-in to a set of trusted accounts.</span></span>
3. <span data-ttu-id="29cac-107">[BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) - 로그인을 사용하지 않도록 설정하거나 사용자가 강제로 로그인해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="29cac-107">[BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) - To disable sign-in or to force users to sign in.</span></span>

