---
title: 사서함 수신 제한 적용
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/31/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13711"
- "9008580"
ms.openlocfilehash: c1ba5ab10b102680cec52f4e0740c3dd2ceaccbd
ms.sourcegitcommit: a36ec7eda49536933dc8c6f9319cf7320e8aa04d
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58829160"
---
# <a name="mailbox-receiving-limit-enforcement"></a>사서함 수신 제한 적용

Microsoft는 최근에 사서함당 메시지 수 임계값을 시간당 3600개로 설정했습니다. 자세한 내용은 [Exchange Online 제한](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-limits)을 참조하세요. 3600개가 넘는 메시지를 받는 Microsoft 365 사서함은 다음 60분 동안 제한됩니다. 

또한 Microsoft 365 사서함에서 받은 메시지를 차단하는 SPR(보낸 사람-수신자 쌍) 제한이 적용됩니다. 단일 보낸 사람이 총 임계값의 33%를 초과하거나 특정 받는 사람에게 시간당 1200개의 메시지를 보내는 경우 SRP 제한이 적용되고, 사서함에서 해당 보낸 사람의 메시지를 더 이상 수락하지 않습니다. 다음 사항에 유의하세요.

- 이 제한은 다른 테넌트, 온-프레미스 또는 인터넷 보낸 사람에게서 받은 전자 메일에 적용됩니다.
- 사서함으로의 전자 메일 배달이 다음 60분 동안 차단됩니다. 
- 이러한 사서함에 메일을 보내는 사람은 사서함이 최대 배달 임계치를 초과했음을 명시하는 배달 못 함 보고서(NDR)(5.2.121 또는 5.2.122)를 받게 됩니다. 인트라 테넌트(동일한 테넌트 내 메일)는 계속해서 배달됩니다.
- SRP 제한이 적용되는 경우 받는 사서함에서 다른 보낸 사람이 보내는 메시지는계속 수락합니다.

관리자는 "수신 제한을 초과하는 사서함"이라는 Exchange 관리 센터에서 새 보고서와 인사이트에 액세스하여 현재 사서함 활동을 모니터링할 수 있습니다. 이 인사이트는 테넌트에 문제가 있는 사서함이 있는 경우에만 표시되지만 보고서는 항상 대시보드에 표시됩니다. 다만 테넌트에 문제가 있는 사서함이 없는 경우 보고서가 빈 페이지로 표시됩니다.

인사이트 수신 제한에 대한 자세한 내용은 [새 EAC의 수신 제한을 초과하는 사서함 인사이트](https://docs.microsoft.com/exchange/monitoring/mail-flow-insights/mailboxes-exceeding-receiving-limits-insights)를 참조하세요.

수신 제함 초과 보고서에 대한 자세한 내용은 [새 EAC의 수신 제한을 초과하는 사서함 보고서](https://docs.microsoft.com/exchange/monitoring/mail-flow-reports/mailboxes-exceeding-receiving-limits-report)를 참조하세요.