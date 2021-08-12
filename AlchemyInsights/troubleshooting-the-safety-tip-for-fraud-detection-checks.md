---
title: 사기 보안 팁 검사에 대한 문제 해결
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: c7ee1fcc887a3221b5f2acda1aa6ae6beb03cb96686d4ecb7828a02f8ff48302
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955972"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>사기 보안 팁 검사에 대한 문제 해결

"보낸 사람이 보안 팁 검색에 실패하여 누구의 신원이 아님"으로 표시되어 있는 경우 보낸 사람이 DKIM 또는 SPF 인증 검사를 통과하지 못했습니다. 이 문제를 해결하는 가장 좋은 방법은 보낸 사람이 직접 승인하는 것입니다. 보낸 사람이 대신 보내고 있는 경우 SPF 레코드에 보낸 사람 IP 주소를 추가하여 승인해야 합니다.
  
자세한 내용은 사기 검색 검사에 대한 보안 팁 (의심스러운) 문제 [해결을](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) 참조하세요.
  
다음은 도움이 될 수 있는 몇 가지 다른 링크입니다.
  
- [Microsoft에서 SPF(보낸 사람 정책 프레임워크)를 사용하여 스푸핑을 방지하는 방법](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [스푸핑을 방지할 수 있도록 SPF 설정](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
