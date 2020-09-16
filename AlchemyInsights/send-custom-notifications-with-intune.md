---
title: Intune을 사용 하 여 사용자 지정 알림 보내기
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
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720652"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>관리 되는 iOS 및 Android 장치의 사용자에 게 사용자 지정 알림을 보내는 방법

Intune에 대 한 사용자 지정 알림은 사용자 장치에서 회사 포털 앱에 의해 처리 됩니다. 그런 다음 앱은 해당 장치에 대 한 푸시 알림을 만듭니다.

다음은 사용자 지정 알림을 수신 하 고 앱이 푸시 알림을 만들도록 지원 하기 위한 장치 필수 구성 요소입니다.

- 장치에 회사 포털 앱이 설치 되어 있어야 합니다.  

- 장치에서 회사 포털 앱이 푸시 알림을 보낼 수 있도록 해야 합니다. 앱이 설치 되거나 업데이트 되 면 사용자에 게 알림을 허용 하 라는 메시지가 표시 됩니다.

- Android 장치에는 Google Play Services가 설치 되어 있어야 합니다.

- 장치는 Intune을 사용 하 여 등록 해야 합니다.

메시지를 보내는 방법 등의 자세한 내용은 [기능 설명서](https://docs.microsoft.com/intune/custom-notifications)를 참조 하십시오.
