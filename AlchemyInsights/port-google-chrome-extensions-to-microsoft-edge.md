---
title: Google Chrome 확장을 Microsoft Edge(Chromium)
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
ms.openlocfilehash: 34ec7e71a2f27eb5b46395876a4d1c903189be1050e523796c9f2a817c20aaa0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973703"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a>Google Chrome 확장을 Microsoft Edge(Chromium)

Google Chrome 확장을 [Microsoft Edge(Chromium) 로 포트할 수 있습니다.](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension) 대부분의 경우 이러한 확장을 실행하려면 최소한의 변경만 Microsoft Edge.

Google Chrome에서 지원하는 확장 API 및 매니페스트 키는 코드와 호환되는 Microsoft Edge. 그러나 Microsoft Edge 확장 API chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken 및 chrome.instanceID를 지원하지 않습니다.