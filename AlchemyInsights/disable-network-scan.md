---
title: 네트워크 검사 사용 안
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001464"
- "3492"
ms.openlocfilehash: 7e67a45b6f4d4b18f47ce55a0fde20f826498c5d25c4a6dec4311d8fe4c3735f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53928555"
---
# <a name="disable-network-scan"></a>네트워크 검사 사용 안

네트워크 공유 검사는 성능에 영향을 줄 수 있습니다.  클라이언트가 기본적으로 네트워크 공유/파일을 검색하지 않도록 설정하려면 Windows Defender 응용 프로그램에서 다음 설정을 **True로 구성합니다.**

- DisableScanningMappedNetworkDrivesForFullScan
- DisableScanningNetworkFiles