---
title: 사용자의 모임 녹음/녹화 차단
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "9325"
ms.openlocfilehash: 3f633ee1fb3329b6fc634acabbc824af1eccfb33
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897979"
---
# <a name="block-user-from-recording-meetings"></a>사용자의 모임 녹음/녹화 차단

특정 사용자가 Teams **모임을** 녹음/녹화하지 못하도록 차단해야 하는 경우 Teams 모임 정책 설정을 통해 녹음/녹화를 차단할 수 있습니다. Microsoft Teams 관리 센터에서 해당  사용자에게 할당된 모임 정책에서 클라우드 녹음/녹화 허용 설정을 해제합니다. 자세한 내용은 [Teams에서 모임 정책 관리를 참조합니다.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording)

특정 사용자가 Teams 모임을 녹음할 수 있도록 허용되거나 기록되지 않는지 확인하기 위해 지원 진단을 사용 합니다. 새 지원 쿼리를 실행하고 **Diag: 모임 녹음/녹화를** 입력합니다. 진단은 지정된 사용자에 대한 정책 설정을 확인하고 해당 정책 설정을 확인합니다. 새 정책 설정이 적용되기까지 몇 시간이 걸릴 수 있으므로 변경한 경우 몇 시간 기다렸다가 진단을 다시 실행해야 합니다.

자세한 내용은 클라우드 [녹음/녹화 켜기 또는 끄기 를 참조하세요.](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording)
