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
# <a name="sign-in-to-microsoft-edge-manually"></a>수동으로 Microsoft Edge에 로그인

첫 실행 경험 중에 사용자가 자동으로 로그인되지 않은 경우 사용자는 브라우저 설정 또는 ID 플라이아웃을 통해 수동으로 로그인할 수 있습니다. 로그인을 관리하기 위해 다음 정책을 사용 합니다.

1. [NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) - 사용자가 Microsoft Edge에서 항상 작업 프로필을 사용할 수 있도록 합니다.
2. [RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) - 로그인을 신뢰할 수 있는 계정 집합으로 제한합니다.
3. [BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) - 로그인을 사용하지 않도록 설정하거나 사용자가 강제로 로그인해야 합니다.

