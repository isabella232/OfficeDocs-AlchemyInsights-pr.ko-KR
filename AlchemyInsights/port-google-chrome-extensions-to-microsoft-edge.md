---
title: Microsoft Edge로 Google Chrome 확장 포트(Chromium)
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
- "9004032"
- "7102"
ms.openlocfilehash: 2a20f258cbcbca7c8db4e38c52464fefb1b6f39d
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49600150"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a><span data-ttu-id="853ec-102">Microsoft Edge로 Google Chrome 확장 포트(Chromium)</span><span class="sxs-lookup"><span data-stu-id="853ec-102">Port Google Chrome extensions to Microsoft Edge (Chromium)</span></span>

<span data-ttu-id="853ec-103">Google Chrome 확장을 [Microsoft Edge(Chromium)로](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension)쉽게 포트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="853ec-103">It's easy to [port Google Chrome extensions to Microsoft Edge (Chromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span></span> <span data-ttu-id="853ec-104">대부분의 경우 Microsoft Edge에서 이러한 확장을 실행하려면 최소한의 변경만 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="853ec-104">In most cases, only minimal changes are needed to run these extensions on Microsoft Edge.</span></span>

<span data-ttu-id="853ec-105">Google Chrome에서 지원하는 확장 API 및 매니페스트 키는 Microsoft Edge와 코드 호환됩니다.</span><span class="sxs-lookup"><span data-stu-id="853ec-105">The extension APIs and manifest keys supported by Google Chrome are code-compatible with Microsoft Edge.</span></span> <span data-ttu-id="853ec-106">그러나 Microsoft Edge는 확장 API chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken 및 chrome.instanceID를 지원하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="853ec-106">However, Microsoft Edge does not support the extension APIs chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken, and chrome.instanceID.</span></span>