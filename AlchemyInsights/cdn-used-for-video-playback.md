---
title: 비디오 재생에 사용되는 CDN
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002552"
- "5146"
ms.openlocfilehash: 6bc87783375a206a84c96eb7ddd58db5bfd31728
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756973"
---
# <a name="cdn-used-for-video-playback"></a>비디오 재생에 사용되는 CDN

Stream 및 외부 앱의 실시간 이벤트 또는 Yammer/Teams의 장치 실시간 이벤트는 자동으로 Azure CDN을 사용합니다. Stream에 업로드된 주문형 비디오는 재생을 위해 아직 Azure CDN을 사용하지 않습니다. Stream의 비 실시간 비디오는 테넌트의 지리적 지역에 있는 테넌트와 연결된 Azure Media Services 원본 서버에서 재생됩니다. 자세한 내용은 다음을 참조하세요.

- [비디오 재생에 사용되는 CDN](https://docs.microsoft.com/stream/network-overview#cdn-used-for-video-playback)
