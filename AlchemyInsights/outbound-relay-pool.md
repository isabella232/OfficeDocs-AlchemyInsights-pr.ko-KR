---
title: 아웃바운드 릴레이 풀
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: d2f83b3afc4abf72a3e18bffe5ac9d6c940cc216916925338c18f0fb8a39948a
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57883137"
---
# <a name="outbound-relay-pool"></a>아웃바운드 릴레이 풀

Microsoft는 사용자 계정을 통해 전자 메일을 릴레이하거나 전달하기 위한 구성을 Microsoft 365. 특정 시나리오의 메시지는 특수 릴레이 풀을 사용하여 Microsoft 365 릴레이됩니다. 릴레이 풀을 사용하여 보낸 메시지는 받는 사람의 정크 메일 폴더에 저장될 수 있습니다. 자세한 내용은 [아웃바운드 배달 풀을 참조하세요.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

릴레이 풀을 사용하는 시나리오를 피하기 위해 전달/릴레이된 메시지가 다음 조건 중 하나를 충족하는지 확인하십시오.

- 아웃바운드 보낸 사람이 테넌트의 허용 도메인입니다.
- SPF(Sender Policy Framework)는 메시지가 전송되면 Microsoft 365.
- P2 보낸 사람 도메인의 DKIM(DomainKeys Identified Mail)은 메시지가 전송될 때 Microsoft 365.
 
위의 조건을 충족하는 메시지는 릴레이 풀을 통해 릴레이되지 않습니다.

도메인의 MX 레코드가 타사 또는 사내 서버를 지정하는 경우 향상된 필터링을 사용하여 SPF 유효성 검사가 인바운드 전자 메일에 대해 올바른지와 릴레이 풀을 통해 전자 메일을 보내지 않도록 합니다.

**릴레이 풀의 영향을 어떻게 알 수 있나요?**

전달되거나 릴레이된 전자 메일이 위의 조건 중 하나를 사용하는 경우 메시지는 릴레이 풀을 통해 릴레이되지 않습니다. 그러나 메시지가 릴레이 풀을 통해 전송되는 경우 아웃바운드 서버 IP는 40.95.0.0/16 범위에 있으며 아웃바운드 서버 이름에 **rly가** 포함됩니다.

