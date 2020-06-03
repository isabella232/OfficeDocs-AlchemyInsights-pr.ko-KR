---
title: 사기 감지 확인을 위한 보안 팁 문제 해결
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 74913492a086de688067d588e95dd87e6946743b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44504989"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>사기 감지 확인을 위한 보안 팁 문제 해결

"보낸 사람이 사기 감지 확인에 실패 하 여 표시 되는 사용자가 아닌 경우" 라는 안전 팁이 나타나면 보낸 사람이 DKIM 또는 SPF 인증 검사를 통과 하지 못한 것입니다. 이 문제를 해결 하는 가장 좋은 방법은 보낸 사람이 자신에 게 권한을 부여 하는 것입니다. 보낸 사람이 사용자를 대신 하 여 보내는 경우에는 SPF 레코드에 보낸 사람의 IP 주소를 추가 하 여 권한을 부여 해야 합니다.
  
자세한 내용은 [사기 검색 검사에 대 한 위험 (의심 스러운) 보안 팁 문제 해결](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) 을 참조 하세요.
  
다음은 도움이 될 수 있는 몇 가지 링크입니다.
  
- [Microsoft가 SPF (sender policy framework)를 사용 하 여 스푸핑을 방지 하는 방법](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [스푸핑을 방지할 수 있도록 SPF 설정](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
