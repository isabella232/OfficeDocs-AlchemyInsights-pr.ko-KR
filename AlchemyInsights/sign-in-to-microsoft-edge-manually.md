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
ms.openlocfilehash: c5d71c26ba3584f8ce496a28587fe75cae2d344f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599512"
---
# <a name="sign-in-to-microsoft-edge-manually"></a>수동으로 Microsoft Edge에 로그인

사용자가 첫 실행 경험 중에 자동으로 로그인되지 않은 경우 사용자는 브라우저 설정 또는 ID 플라이아웃을 통해 수동으로 로그인할 수 있습니다. 로그인을 관리하기 위해 다음 정책을 사용 합니다.

1. [NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) - 사용자가 Microsoft Edge에서 항상 작업 프로필을 사용할 수 있도록 합니다.
2. [RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) - 신뢰할 수 있는 계정 집합으로 로그인을 제한합니다.
3. [BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) - 로그인을 사용하지 않도록 설정하거나 사용자가 강제로 로그인을 하게 하세요.

