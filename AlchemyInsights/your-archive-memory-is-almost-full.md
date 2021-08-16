---
title: 보관 사서함이 거의 가득 차 있습니다.
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 085d9b211d5a8e9a0e1eb12af14d87a4e59c844a3afa012095dfd60db316ad14
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046758"
---
# <a name="your-archive-mailbox-is-almost-full"></a>보관 사서함이 거의 가득 차 있습니다.

사용자가 경고를 받는 경우 **보관 사서함이 거의 가득 차거나** 보관 사서함의 크기를 늘려야 합니다. 몇 가지 팁은 다음과 같습니다.

1. 사용자에게 Exchange Online 계획 1이 할당된 경우 Exchange Online **Plan 2** 라이선스로 업그레이드하여 크기를 50GB에서 100GB로 늘입니다.
1. 사용자에게 Exchange Online 계획 **2** 또는 Exchange Online 추가 기능을 사용하는 Exchange Online 계획 Exchange Online Archiving 1이 이미 할당되어 있는 경우 다음 단계를 사용하여 자동 확장 보관을 사용하도록 설정하십시오.
 
    1. [커넥트 Powershell을 Exchange Online 합니다.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)
    2. 사용자에 대해 다음 commandlet을 실행합니다.  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. 다음 commandlet을 실행하여 사용자가 사용할 수 있도록 설정되어 있는지 확인합니다.  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

자세한 내용은 다음을 참조하십시오:

- [무제한 보관 사용 - 관리자 도움말 - Microsoft 365 준수 | Microsoft Docs](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online 제한 - 서비스 설명 | Microsoft Docs](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [다른 비즈니스 계획 계획 | Microsoft Docs](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

