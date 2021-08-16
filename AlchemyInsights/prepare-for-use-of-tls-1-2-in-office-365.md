---
title: Microsoft 365에서 TLS 1.2 사용 준비
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Critical
ms.custom:
- "1266"
- "1600052"
ms.assetid: d5c84f5c-a3ca-4abd-8633-7e9ff01328a9
ms.openlocfilehash: 79a9dc3833f8329adeb24d27014d08c14eb93d1f5f840c5cfa2ce10991107b1c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040404"
---
# <a name="prepare-for-use-of-tls-12-in-microsoft-365"></a>Microsoft 365에서 TLS 1.2 사용 준비

2018년 10월 31일부터 Microsoft 365가 TLS 1.2로 계속해서 전환됩니다. 2020년 10월 15일부터 O365는 서비스 전반에서 TLS 1.0 및 1.1의 비호출을 시작합니다. 이러한 변경에 대한 배포는 향후 몇 주 및 몇 개월 동안 계속될 것이지만, 고객은 2020년 10월 15일부터 O365에 참여할 때 TLS 1.0/1.1 호출이 작동하지 않을 것으로 가정해야 합니다. 앞서 전달된 대로(2017년 12월 MC126199, 2018년 2월 MC128929, 2019년 7월 MC186827, 2020년 7월 MC218794) 모든 온라인 서비스를 TLS(전송 계층 보안) 1.2+로 전환하여 동급 최강의 암호화를 제공하고, 기본적으로 서비스의 보안을 강화하고 있습니다. 고객은 서버 및 리소스에 TLS 1.0/1.1을 계속 사용할 수 있지만 O365 리소스와 상호 작용할 때는 TLS 1.2 이상만 작동한다고 가정해야 합니다.
  
이러한 변경 사항에 대한 자세한 내용은 [여기](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) 및 [여기](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide)를 참조하시기 바랍니다.

  