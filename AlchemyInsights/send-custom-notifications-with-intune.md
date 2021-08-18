---
title: Intune을 사용하여 사용자 지정 알림 보내기
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 58acaa29f9d0b066cc7be6f6ee57b1806d0e8812b194e20166b133b7715226a8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086170"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>관리되는 iOS 및 Android 장치의 사용자에게 사용자 지정 알림을 보내는 방법

Intune에 대한 사용자 지정 알림은 사용자 회사 포털 앱에 의해 처리됩니다. 그런 다음 앱은 해당 디바이스에 푸시 알림을 만듭니다.

다음은 사용자 지정 알림 수신을 지원하기 위한 장치 선행 사항으로, 앱이 푸시 알림을 만들 수 있는 경우입니다.

- 디바이스에 앱 앱이 회사 포털 있어야 합니다.  

- 디바이스는 앱이 푸시 회사 포털 보낼 수 있도록 허용해야 합니다. 앱이 설치 또는 업데이트되면 사용자에게 알림을 허용하라는 메시지가 표시됩니다.

- Android 장치에는 Google Play Services가 설치되어 있어야 합니다.

- 디바이스를 Intune에 등록해야 합니다.

메시지를 보내는 방법을 비롯한 자세한 내용은 기능 [설명서를 참조하십시오.](https://docs.microsoft.com/intune/custom-notifications)
