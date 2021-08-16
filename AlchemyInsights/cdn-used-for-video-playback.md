---
title: 비디오 재생에 사용되는 CDN
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002552"
- "5146"
ms.openlocfilehash: 399be421994437d4cd2df644531334c58d177ec3293e7e379d84cd8326823a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54071122"
---
# <a name="cdn-used-for-video-playback"></a>비디오 재생에 사용되는 CDN

Stream 및 외부 앱의 실시간 이벤트 또는 Yammer/Teams의 장치 실시간 이벤트는 자동으로 Azure CDN을 사용합니다. Stream에 업로드된 주문형 비디오는 재생을 위해 아직 Azure CDN을 사용하지 않습니다. Stream의 비 실시간 비디오는 테넌트의 지리적 지역에 있는 테넌트와 연결된 Azure Media Services 원본 서버에서 재생됩니다. 자세한 내용은 다음을 참조하세요.

- [비디오 재생에 사용되는 CDN](https://docs.microsoft.com/stream/network-overview#cdn-used-for-video-playback)
