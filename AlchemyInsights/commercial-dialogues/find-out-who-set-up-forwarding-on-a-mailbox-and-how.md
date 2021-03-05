---
title: 사서함에 대해 전달을 설정하는 사람 및 방법 확인
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464870"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>사서함에 대해 전달을 설정하는 사람 및 방법 확인

외부 전달이 사서함에 설정된 경우 활동은 사서함 cmdlet의 일부로 Set-Mailbox 감사됩니다. 감사 로그에서 활동을 찾는 방법에는 다음이 있습니다.

1. [Office 365 보안](https://go.microsoft.com/fwlink/p/?linkid=2077143)및 준수 & 로 이동 합니다.
1. 감사 **로그** >  **검색 검색을 선택합니다.**
    > [!NOTE]
    > 감사를 켜야 하는 알림이 표시된 경우 지금 진행하여 켜야 합니다. 이 기능을 설정하지 않은 경우 검색 결과에서 이전 날짜의 데이터를 끌 수 없습니다.
1. 활동 **필드가** 모든 활동에 대한 결과 표시(기본값)로 **설정되어** 있는지 확인 날짜 범위를 지정합니다. 사용자 이름을 지정할 필요가 없습니다.
1. 검색 **을 선택합니다.** 활동은 결과 아래에 **표시됩니다.**
1. 필터 **결과 를** 선택한 다음 활동 필터 필드에 **Set-mailbox를** 입력합니다.  그러면 모든 **Set-Mailbox 활동이 반환됩니다.**
1. 세부 정보를 확인하려면 활동을 선택한 다음 추가 정보 **를 선택합니다.** 매개 **변수에서** 사서함에 설정된 전달 전자 메일 주소를 볼 수 있습니다. **UserID는** 사서함에 외부 전달을 설정한 사용자를 나타내며,
자세한 내용은 [Office 365](https://go.microsoft.com/fwlink/?linkid=2103944)감사 로그 검색을 참조하여 일반적인 시나리오 문제를 해결합니다.