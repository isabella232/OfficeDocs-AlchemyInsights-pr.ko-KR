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
- "8297"
- "9004617"
ms.openlocfilehash: 1c71d74d01c1e38e4c7789aea2c0b43701b3a5de
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505290"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a>Microsoft Edge로 Google Chrome 확장 포트(Chromium)

Google Chrome 확장을 [Microsoft Edge(Chromium)로](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension)쉽게 포트할 수 있습니다. 대부분의 경우 Microsoft Edge에서 이러한 확장을 실행하려면 최소한의 변경만 필요합니다.

Google Chrome에서 지원하는 확장 API 및 매니페스트 키는 Microsoft Edge와 코드 호환됩니다. 그러나 Microsoft Edge는 확장 API chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken 및 chrome.instanceID를 지원하지 않습니다.