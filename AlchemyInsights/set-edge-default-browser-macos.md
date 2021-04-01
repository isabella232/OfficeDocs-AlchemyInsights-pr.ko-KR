---
title: macOS 장치에서 Microsoft Edge를 기본 브라우저로 설정
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
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426821"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a><span data-ttu-id="f0666-102">macOS 장치에서 Microsoft Edge를 기본 브라우저로 설정</span><span class="sxs-lookup"><span data-stu-id="f0666-102">Set Microsoft Edge as the default browser on a macOS device</span></span>

<span data-ttu-id="f0666-103">다음 두 가지 방법 중 하나를 사용하여 Microsoft Edge를 기본 브라우저로 설정하세요.</span><span class="sxs-lookup"><span data-stu-id="f0666-103">Use one of these two methods to set Microsoft Edge as the default browser:</span></span>

<span data-ttu-id="f0666-104">방법 1: Microsoft Edge가 이미 기본 브라우저로 설정된 MacOS 이미지로 장치를 플래시합니다.</span><span class="sxs-lookup"><span data-stu-id="f0666-104">Method 1: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span></span>

<span data-ttu-id="f0666-105">방법 2: 기본 브라우저 설정 사용 정책을 설정하여 사용자에게 Microsoft Edge를 기본 브라우저로 설정하라는 메시지를 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="f0666-105">Method 2: Set the DefaultBrowserSettingEnabled policy to prompt the user to set Microsoft Edge as the default browser.</span></span>

<span data-ttu-id="f0666-106">두 방법 중 하나를 통해 사용자가 기본 브라우저를 변경할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f0666-106">Either method allows a user to change the default browser.</span></span> <span data-ttu-id="f0666-107">따라서 방법 1을 사용한 경우에도 기본 브라우저 설정 사용 정책을 배포하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="f0666-107">For this reason, we recommend that you deploy the DefaultBrowserSettingEnabled policy even if you used method 1.</span></span> <span data-ttu-id="f0666-108">정책 배포 후 사용자가 기본 브라우저를 변경하면 기본 브라우저를 다시 Microsoft Edge로 설정하라는 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="f0666-108">If a user changes the default browser after the policy is deployed, the policy prompts the user to set the default browser back to Microsoft Edge.</span></span>
