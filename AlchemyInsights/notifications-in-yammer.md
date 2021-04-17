---
title: Yammer의 알림
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
- "9002878"
- "5480"
ms.openlocfilehash: 8e7c03f2b557a7d3c409b2ee418df055d0569ee6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833585"
---
# <a name="notifications-in-yammer"></a>Yammer의 알림

관련 대화에서 새 활동에 대해 알리기 위해 [Yammer의 알림 전송](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996)은 전자 메일을 통하거나, 혹은 모바일 장치에서 Yammer를 사용하는 경우에는 푸시 알림을 통해 수행됩니다. 기본적으로 Yammer는 다양한 유형의 활동에 대한 알림을 사용자의 네트워크에서 보냅니다. 사용자는 Yammer 웹 사이트를 통해 전자 메일 설정을 업데이트할 수 있고, 푸시 알람은 모바일 앱을 통해 구성됩니다. 

Yammer가 [Outlook의 대화형 전자 메일](https://techcommunity.microsoft.com/t5/outlook-blog/interactive-yammer-emails-in-outlook-on-the-web-are-here/ba-p/1209420)에 대한 지원을 추가했습니다. 일부 전자 메일(메시지 복사본)은 웹용 Outlook에서 대화형이 됩니다. 향후 업데이트에서는 이를 다른 버전의 Outlook으로 가져올 것입니다.

**Yammer의 알림 유형**

- 전자 메일(그룹에서의 업데이트, 사용자를 그룹에 초대 시, 사용자의 받은 편지함에 메시지를 받는 경우 등)
- 푸시 알림(사용자가 멘션된 경우, 모바일 장치로 전송되어 받은 편지함에 메시지를 받게되는 경우 등)
- 바탕 화면 팝업(Yammer 데스크톱 앱이 설치되어 있는 경우 "토스트" 알림이라는 알림이 사용자에게 표시됩니다.)
- 벨 알림(Yammer 웹 사이트 내에서, 사용자에게 다양한 이벤트에 대한 알림이 표시됩니다. 이러한 알림에 항상 연결된 전자 메일 또는 푸시 알림이 있지는 않습니다.)

더 많은 [알림에 대한 상세한 정보](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996)를 사용할 수 있습니다.

**알림 관리**

사용자는 자신의 알림을 직접 관리해야 합니다. [Yammer 전자 메일 및 모바일 알림을 설정 및 해제하는 방법](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996)에 대한 정보를 확인할 수 있습니다. 

관리자가 사용자를 대신하여 모든 알림을 해제하거나 알림을 제어할 수 없습니다. 관리자는 [전자 메일에 포함된 로고와 사용자가 전자 메일로 게시된 메시지를 확인해야 하는지의 여부를 컨트롤](https://docs.microsoft.com/yammer/configure-your-yammer-network/configure-email-and-yammer)할 수 있습니다.

**조직의 여러 사용자에게 전송되는 전자 메일 알림**

간혹 Yammer에서 하나의 전자 메일 알림을 보낼 때 예상보다 많은 사용자가 이 알림을 받게 됩니다. 이는 배포 목록 또는 다른 유형의 비개별 전자 메일 주소가 Yammer에 추가되는 경우 발생합니다. Yammer는 모든 경우에 전자 메일 주소가 단일 사용자에 속하는지 또는 전자 메일 주소가 하나의 전자 메일을 여러 명의 받는 사람에게 전달하는 전자 메일 주소인지 알지 못합니다. 이 문제가 발생하면 Yammer에서 [해당 전자 메일 주소를 사용하여 잘못된 사용자를 일시 중단(비활성화)](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)하는 조치를 취해야 합니다. 

이 문제 발생의 확률을 줄이려면 다음을 수행합니다.

1. Yammer에 [Office 365 ID 적용](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. 조직에 전자 메일을 보내지 못하도록 외부의 보낸 사람을 차단하거나, 보낸 사람을 승인된 목록으로 제한합니다.

이 문제가 발생하는 경우 다음을 수행합니다.

1. Yammer의 사용자와 일치하는 전자 메일의 받는 사람을 확인합니다. 예를 들어 all-in-sales@fabrikam.com는 모든 영업 직원에 대한 DL입니다. 이 DL은 사용자가 받은 Yammer 전자 메일에서 식별할 수 있습니다.
2. All-in-sales@fabrikam.com 전자 메일 주소가 있는 사용자를 일시 중지하려면 [네트워크 관리자의 비활성화(일시 중지) 기능](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)을 사용합니다. 일시 중지는 취소할 수 있으므로 삭제보다 안전합니다. 사용자 삭제는 90일 후에 자동으로 수행됩니다.
3. 원하는 경우 [사용자 내보내기](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data#ExportUsers)를 검토하여 일시 중단 해야 하는 기타 비사용자의 전자 메일 주소를 확인합니다.
